# Comparing `tmp/gdsfactory-6.95.0.tar.gz` & `tmp/gdsfactory-6.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.95.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-6.96.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-6.95.0.tar` & `gdsfactory-6.96.0.tar`

### file list

```diff
@@ -1,693 +1,693 @@
--rw-r--r--   0        0        0     1072 2023-05-18 23:12:36.028450 gdsfactory-6.95.0/LICENSE
--rw-r--r--   0        0        0    14319 2023-05-18 23:12:36.028450 gdsfactory-6.95.0/README.md
--rw-r--r--   0        0        0     3566 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15639 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/asserts.py
--rw-r--r--   0        0        0    12272 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/cell.py
--rw-r--r--   0        0        0    16040 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5718 2023-05-18 23:12:36.036450 gdsfactory-6.95.0/gdsfactory/cli.py
--rw-r--r--   0        0        0   102023 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/component.py
--rw-r--r--   0        0        0    23424 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29879 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7903 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3664 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9876 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-18 23:12:36.040450 gdsfactory-6.95.0/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7988 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7221 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4960 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1578 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8811 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7501 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     3846 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2740 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16692 2023-05-18 23:12:36.044450 gdsfactory-6.95.0/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2526 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7730 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3160 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15612 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4430 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     8145 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/containers.py
--rw-r--r--   0        0        0    82893 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2982 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/decorators.py
--rw-r--r--   0        0        0     7312 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/difftest.py
--rw-r--r--   0        0        0     1020 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/events.py
--rw-r--r--   0        0        0      204 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     1940 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     7445 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/export/write_gerbers.py
--rw-r--r--   0        0        0     2976 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11890 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6193 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-05-18 23:12:36.048451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10704 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4337 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4311 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1854 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1883 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5015 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7084 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3054 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4812 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     1898 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10532 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23569 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14446 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9745 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/grid.py
--rw-r--r--   0        0        0     4393 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/install.py
--rw-r--r--   0        0        0     1970 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/name.py
--rw-r--r--   0        0        0    11586 2023-05-18 23:12:36.052451 gdsfactory-6.95.0/gdsfactory/pack.py
--rw-r--r--   0        0        0    50930 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/path.py
--rw-r--r--   0        0        0    27295 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6220 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0       32 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/__init__.py
--rw-r--r--   0        0        0     4080 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/main.py
--rwxr-xr-x   0        0        0     7511 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/server.py
--rwxr-xr-x   0        0        0      594 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/plugins/web/static/client.css
--rw-r--r--   0        0        0    32235 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/port.py
--rw-r--r--   0        0        0    37817 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38948 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8652 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6910 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10872 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-18 23:12:36.056451 gdsfactory-6.95.0/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4379 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2897 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1109 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1062 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2100 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1839 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1592 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1577 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4313 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4271 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2171 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17862 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23687 2023-05-18 23:12:36.060451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19756 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1644 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1787 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2221 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3455 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     2003 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15915 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18182 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12312 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    14053 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21281 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8143 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9577 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11824 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2513 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16334 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1624 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-18 23:12:36.064451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21071 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    27469 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0      744 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1270 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    10515 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16091 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2368 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1618 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4166 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2773 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8924 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4458 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2728 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7148 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5411 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     8023 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1137 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      649 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15492 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1169 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3069 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      703 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4685 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6800 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13894 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2225 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-18 23:12:36.068451 gdsfactory-6.95.0/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1405 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7789 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7607 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    16139 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42133 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/types.py
--rw-r--r--   0        0        0    10008 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1342 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      684 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1453 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4865 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7969 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7480 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5687 2023-05-18 23:12:36.072451 gdsfactory-6.95.0/pyproject.toml
--rw-r--r--   0        0        0    18772 1970-01-01 00:00:00.000000 gdsfactory-6.95.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-19 04:20:22.281426 gdsfactory-6.96.0/LICENSE
+-rw-r--r--   0        0        0    14319 2023-05-19 04:20:22.281426 gdsfactory-6.96.0/README.md
+-rw-r--r--   0        0        0     3566 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15639 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    12272 2023-05-19 04:20:22.289426 gdsfactory-6.96.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    16040 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5718 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   102063 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23424 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29879 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7903 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3664 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9876 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-19 04:20:22.293426 gdsfactory-6.96.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7988 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7221 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4960 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1578 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8811 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2814 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3299 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7579 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     3846 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2740 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5267 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-19 04:20:22.297427 gdsfactory-6.96.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16692 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2526 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7730 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2457 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1215 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3821 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3160 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15612 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4430 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     8145 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    82893 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2982 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     7312 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0     1020 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      204 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     1940 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     7445 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/export/write_gerbers.py
+-rw-r--r--   0        0        0     2976 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11890 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1059 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6193 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-05-19 04:20:22.301427 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10704 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4337 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4311 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1854 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1883 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5015 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7084 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3054 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4812 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     1898 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10532 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23569 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14446 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9745 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4393 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1970 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11586 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    50930 2023-05-19 04:20:22.305426 gdsfactory-6.96.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    27294 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6220 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0       32 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/__init__.py
+-rw-r--r--   0        0        0     4080 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/main.py
+-rwxr-xr-x   0        0        0     7511 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/server.py
+-rwxr-xr-x   0        0        0      594 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/plugins/web/static/client.css
+-rw-r--r--   0        0        0    32235 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37817 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38948 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8652 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6910 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9233 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10872 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34394 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4379 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-19 04:20:22.309427 gdsfactory-6.96.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2897 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1109 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      507 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      493 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1062 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2140 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1879 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1632 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1617 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4497 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4455 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2231 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17862 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4194 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      547 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    23687 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19756 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1644 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1787 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2221 2023-05-19 04:20:22.313427 gdsfactory-6.96.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3455 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     2003 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15915 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18182 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12312 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    14053 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21281 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8143 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9577 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11824 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2513 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16334 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1624 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21071 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     2821 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    27439 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-19 04:20:22.317427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0      744 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1270 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10515 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16091 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2368 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4166 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2773 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8924 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4458 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2728 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7148 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5411 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     8023 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1137 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      649 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15492 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1169 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3069 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      703 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4685 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6800 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13894 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2225 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1405 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-19 04:20:22.321427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7789 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7607 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    16139 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42133 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10008 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1342 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      684 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1453 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4865 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7969 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7480 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     5687 2023-05-19 04:20:22.325427 gdsfactory-6.96.0/pyproject.toml
+-rw-r--r--   0        0        0    18772 1970-01-01 00:00:00.000000 gdsfactory-6.96.0/PKG-INFO
```

### Comparing `gdsfactory-6.95.0/LICENSE` & `gdsfactory-6.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/README.md` & `gdsfactory-6.96.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.95.0
+# gdsfactory 6.96.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

### Comparing `gdsfactory-6.95.0/gdsfactory/__init__.py` & `gdsfactory-6.96.0/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,8 @@
     "snap",
     "typings",
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
-__version__ = "6.95.0"
+__version__ = "6.96.0"
```

### Comparing `gdsfactory-6.95.0/gdsfactory/add_keepout.py` & `gdsfactory-6.96.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_labels.py` & `gdsfactory-6.96.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_loopback.py` & `gdsfactory-6.96.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_padding.py` & `gdsfactory-6.96.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_pins.py` & `gdsfactory-6.96.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_ports.py` & `gdsfactory-6.96.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_tapers.py` & `gdsfactory-6.96.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.96.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/add_termination.py` & `gdsfactory-6.96.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/asserts.py` & `gdsfactory-6.96.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/cell.py` & `gdsfactory-6.96.0/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/circuitviz.py` & `gdsfactory-6.96.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/cli.py` & `gdsfactory-6.96.0/gdsfactory/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.95.0"
+VERSION = "6.96.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.95.0/gdsfactory/component.py` & `gdsfactory-6.96.0/gdsfactory/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -6218,17 +6218,17 @@
 00018490: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
 000184a0: 7472 6169 6768 7428 6c61 7965 723d 2832  traight(layer=(2
 000184b0: 2c20 3029 290a 2020 2020 7265 6d61 7020  , 0)).    remap 
 000184c0: 3d20 632e 7265 6d61 705f 6c61 7965 7273  = c.remap_layers
 000184d0: 286c 6179 6572 6d61 703d 7b28 322c 2030  (layermap={(2, 0
 000184e0: 293a 2067 662e 4c41 5945 522e 5747 4e7d  ): gf.LAYER.WGN}
 000184f0: 290a 2020 2020 6861 7368 5f67 656f 6d65  ).    hash_geome
-00018500: 7472 7920 3d20 2238 3366 6263 3661 3832  try = "83fbc6a82
-00018510: 3839 3530 3565 6165 6433 6132 6533 6162  89505eaed3a2e3ab
-00018520: 3237 3963 6330 3366 3565 3464 3030 6322  279cc03f5e4d00c"
+00018500: 7472 7920 3d20 2233 3263 6431 3465 6137  try = "32cd14ea7
+00018510: 6365 3133 6366 3166 3433 3032 3737 6234  ce13cf1f430277b4
+00018520: 3530 3534 6130 6137 3930 3961 3363 3422  5054a0a7909a3c4"
 00018530: 0a0a 2020 2020 6173 7365 7274 2028 0a20  ..    assert (. 
 00018540: 2020 2020 2020 2072 656d 6170 2e68 6173         remap.has
 00018550: 685f 6765 6f6d 6574 7279 2829 203d 3d20  h_geometry() == 
 00018560: 6861 7368 5f67 656f 6d65 7472 790a 2020  hash_geometry.  
 00018570: 2020 292c 2066 2268 6173 685f 6765 6f6d    ), f"hash_geom
 00018580: 6574 7279 203d 207b 7265 6d61 702e 6861  etry = {remap.ha
 00018590: 7368 5f67 656f 6d65 7472 7928 2921 727d  sh_geometry()!r}
@@ -6329,49 +6329,51 @@
 00018b80: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
 00018b90: 616d 6529 0a20 2020 2072 756e 5f78 6f72  ame).    run_xor
 00018ba0: 2869 6e76 616c 6964 5f72 6566 735f 6669  (invalid_refs_fi
 00018bb0: 6c65 6e61 6d65 2c20 696e 7661 6c69 645f  lename, invalid_
 00018bc0: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
 00018bd0: 616d 6529 0a0a 0a69 6620 5f5f 6e61 6d65  ame)...if __name
 00018be0: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00018bf0: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
-00018c00: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
-00018c10: 2020 2063 203d 2067 662e 436f 6d70 6f6e     c = gf.Compon
-00018c20: 656e 7428 290a 2020 2020 7020 3d20 632e  ent().    p = c.
-00018c30: 6164 645f 706f 6c79 676f 6e28 0a20 2020  add_polygon(.   
-00018c40: 2020 2020 205b 282d 382c 2036 2c20 372c       [(-8, 6, 7,
-00018c50: 2039 292c 2028 2d36 2c20 382c 2031 372c   9), (-6, 8, 17,
-00018c60: 2035 295d 2c20 6c61 7965 723d 2831 2c20   5)], layer=(1, 
-00018c70: 3029 0a20 2020 2029 2020 2320 4744 5320  0).    )  # GDS 
-00018c80: 6c61 7965 7273 2061 7265 2074 7570 6c65  layers are tuple
-00018c90: 7320 6f66 2069 6e74 7320 2862 7574 2069  s of ints (but i
-00018ca0: 6620 7765 2075 7365 206f 6e6c 7920 6f6e  f we use only on
-00018cb0: 6520 6e75 6d62 6572 2069 7420 6173 7375  e number it assu
-00018cc0: 6d65 7320 7468 6520 6f74 6865 7220 6e75  mes the other nu
-00018cd0: 6d62 6572 2069 7320 3029 0a0a 2020 2020  mber is 0)..    
-00018ce0: 2320 6332 203d 2067 662e 436f 6d70 6f6e  # c2 = gf.Compon
-00018cf0: 656e 7428 290a 2020 2020 6320 3d20 6766  ent().    c = gf
-00018d00: 2e63 6f6d 706f 6e65 6e74 732e 6d7a 6928  .components.mzi(
-00018d10: 290a 2020 2020 7072 696e 7428 632e 6765  ).    print(c.ge
-00018d20: 745f 6c61 7965 725f 6e61 6d65 7328 2929  t_layer_names())
-00018d30: 0a20 2020 2023 2063 203d 2067 662e 636f  .    # c = gf.co
-00018d40: 6d70 6f6e 656e 7473 2e6d 7a69 2829 0a20  mponents.mzi(). 
-00018d50: 2020 2023 2070 7269 6e74 2863 2e67 6574     # print(c.get
-00018d60: 5f6c 6179 6572 5f6e 616d 6573 2829 290a  _layer_names()).
-00018d70: 2020 2020 2320 7220 3d20 632e 7265 6628      # r = c.ref(
-00018d80: 290a 2020 2020 2320 6332 2e63 6f70 795f  ).    # c2.copy_
-00018d90: 6368 696c 645f 696e 666f 2863 2e6e 616d  child_info(c.nam
-00018da0: 6564 5f72 6566 6572 656e 6365 735b 2273  ed_references["s
-00018db0: 7874 225d 290a 2020 2020 2320 7465 7374  xt"]).    # test
-00018dc0: 5f72 656d 6170 5f6c 6179 6572 7328 290a  _remap_layers().
-00018dd0: 2020 2020 2320 6320 3d20 7465 7374 5f67      # c = test_g
-00018de0: 6574 5f6c 6179 6572 7328 290a 2020 2020  et_layers().    
-00018df0: 2320 632e 706c 6f74 5f71 7428 290a 2020  # c.plot_qt().  
-00018e00: 2020 2320 632e 706c 6f74 6828 290a 2020    # c.ploth().  
-00018e10: 2020 2320 6320 3d20 7465 7374 5f65 7874    # c = test_ext
-00018e20: 7261 6374 2829 0a20 2020 2023 2067 6473  ract().    # gds
-00018e30: 7061 7468 203d 2063 2e77 7269 7465 5f67  path = c.write_g
-00018e40: 6473 2829 0a20 2020 2023 2067 662e 7368  ds().    # gf.sh
-00018e50: 6f77 2867 6473 7061 7468 290a 2020 2020  ow(gdspath).    
-00018e60: 2320 632e 7368 6f77 2873 686f 775f 706f  # c.show(show_po
-00018e70: 7274 733d 5472 7565 290a 2020 2020 632e  rts=True).    c.
-00018e80: 7368 6f77 2829 0a                        show().
+00018bf0: 3a0a 2020 2020 2320 696d 706f 7274 2067  :.    # import g
+00018c00: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
+00018c10: 0a20 2020 2074 6573 745f 7265 6d61 705f  .    test_remap_
+00018c20: 6c61 7965 7273 2829 0a20 2020 2023 2063  layers().    # c
+00018c30: 203d 2067 662e 436f 6d70 6f6e 656e 7428   = gf.Component(
+00018c40: 290a 2020 2020 2320 7020 3d20 632e 6164  ).    # p = c.ad
+00018c50: 645f 706f 6c79 676f 6e28 0a20 2020 2023  d_polygon(.    #
+00018c60: 2020 2020 205b 282d 382c 2036 2c20 372c       [(-8, 6, 7,
+00018c70: 2039 292c 2028 2d36 2c20 382c 2031 372c   9), (-6, 8, 17,
+00018c80: 2035 295d 2c20 6c61 7965 723d 2831 2c20   5)], layer=(1, 
+00018c90: 3029 0a20 2020 2023 2029 2020 2320 4744  0).    # )  # GD
+00018ca0: 5320 6c61 7965 7273 2061 7265 2074 7570  S layers are tup
+00018cb0: 6c65 7320 6f66 2069 6e74 7320 2862 7574  les of ints (but
+00018cc0: 2069 6620 7765 2075 7365 206f 6e6c 7920   if we use only 
+00018cd0: 6f6e 6520 6e75 6d62 6572 2069 7420 6173  one number it as
+00018ce0: 7375 6d65 7320 7468 6520 6f74 6865 7220  sumes the other 
+00018cf0: 6e75 6d62 6572 2069 7320 3029 0a0a 2020  number is 0)..  
+00018d00: 2020 2320 6332 203d 2067 662e 436f 6d70    # c2 = gf.Comp
+00018d10: 6f6e 656e 7428 290a 2020 2020 2320 6320  onent().    # c 
+00018d20: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
+00018d30: 6d7a 6928 290a 2020 2020 2320 7072 696e  mzi().    # prin
+00018d40: 7428 632e 6765 745f 6c61 7965 725f 6e61  t(c.get_layer_na
+00018d50: 6d65 7328 2929 0a20 2020 2023 2063 203d  mes()).    # c =
+00018d60: 2067 662e 636f 6d70 6f6e 656e 7473 2e6d   gf.components.m
+00018d70: 7a69 2829 0a20 2020 2023 2070 7269 6e74  zi().    # print
+00018d80: 2863 2e67 6574 5f6c 6179 6572 5f6e 616d  (c.get_layer_nam
+00018d90: 6573 2829 290a 2020 2020 2320 7220 3d20  es()).    # r = 
+00018da0: 632e 7265 6628 290a 2020 2020 2320 6332  c.ref().    # c2
+00018db0: 2e63 6f70 795f 6368 696c 645f 696e 666f  .copy_child_info
+00018dc0: 2863 2e6e 616d 6564 5f72 6566 6572 656e  (c.named_referen
+00018dd0: 6365 735b 2273 7874 225d 290a 2020 2020  ces["sxt"]).    
+00018de0: 2320 7465 7374 5f72 656d 6170 5f6c 6179  # test_remap_lay
+00018df0: 6572 7328 290a 2020 2020 2320 6320 3d20  ers().    # c = 
+00018e00: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
+00018e10: 290a 2020 2020 2320 632e 706c 6f74 5f71  ).    # c.plot_q
+00018e20: 7428 290a 2020 2020 2320 632e 706c 6f74  t().    # c.plot
+00018e30: 6828 290a 2020 2020 2320 6320 3d20 7465  h().    # c = te
+00018e40: 7374 5f65 7874 7261 6374 2829 0a20 2020  st_extract().   
+00018e50: 2023 2067 6473 7061 7468 203d 2063 2e77   # gdspath = c.w
+00018e60: 7269 7465 5f67 6473 2829 0a20 2020 2023  rite_gds().    #
+00018e70: 2067 662e 7368 6f77 2867 6473 7061 7468   gf.show(gdspath
+00018e80: 290a 2020 2020 2320 632e 7368 6f77 2873  ).    # c.show(s
+00018e90: 686f 775f 706f 7274 733d 5472 7565 290a  how_ports=True).
+00018ea0: 2020 2020 2320 632e 7368 6f77 2829 0a        # c.show().
```

### Comparing `gdsfactory-6.95.0/gdsfactory/component_layout.py` & `gdsfactory-6.96.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/component_reference.py` & `gdsfactory-6.96.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/C.py` & `gdsfactory-6.96.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/L.py` & `gdsfactory-6.96.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/__init__.py` & `gdsfactory-6.96.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.96.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.96.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/add_trenches.py` & `gdsfactory-6.96.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/align.py` & `gdsfactory-6.96.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/array_component.py` & `gdsfactory-6.96.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.96.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/array_with_via.py` & `gdsfactory-6.96.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/awg.py` & `gdsfactory-6.96.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bbox.py` & `gdsfactory-6.96.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bend_circular.py` & `gdsfactory-6.96.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.96.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bend_euler.py` & `gdsfactory-6.96.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bend_port.py` & `gdsfactory-6.96.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bend_s.py` & `gdsfactory-6.96.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/bezier.py` & `gdsfactory-6.96.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cavity.py` & `gdsfactory-6.96.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdc.py` & `gdsfactory-6.96.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.96.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.96.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.96.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.96.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.96.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/circle.py` & `gdsfactory-6.96.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.96.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.96.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.96.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.96.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/compass.py` & `gdsfactory-6.96.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/component_lattice.py` & `gdsfactory-6.96.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/component_sequence.py` & `gdsfactory-6.96.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/copy_layers.py` & `gdsfactory-6.96.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler90.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_full.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.96.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cross.py` & `gdsfactory-6.96.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.96.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.96.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.96.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.96.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cutback_component.py` & `gdsfactory-6.96.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.96.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/dbr.py` & `gdsfactory-6.96.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.96.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/delay_snake.py` & `gdsfactory-6.96.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.96.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.96.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.96.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.96.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/die.py` & `gdsfactory-6.96.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/die_bbox.py` & `gdsfactory-6.96.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.96.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/disk.py` & `gdsfactory-6.96.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.96.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ellipse.py` & `gdsfactory-6.96.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.96.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/extension.py` & `gdsfactory-6.96.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/fiber.py` & `gdsfactory-6.96.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/fiber_array.py` & `gdsfactory-6.96.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.96.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.96.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.96.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/greek_cross.py` & `gdsfactory-6.96.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/hline.py` & `gdsfactory-6.96.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.96.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.96.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.96.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/litho_steps.py` & `gdsfactory-6.96.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/logo.py` & `gdsfactory-6.96.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.96.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.96.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.96.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.96.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.96.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.96.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mode_converter.py` & `gdsfactory-6.96.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,16 @@
 
     c = mzi(cross_section="strip")
     # c = gf.components.mzi2x2_2x2(straight_x_top="straight_heater_metal")
     # c.show(show_ports=True)
 
     # c = gf.components.mzi2x2_2x2(straight_x_top="straight_heater_metal")
     c = gf.routing.add_fiber_array(c)
+    # gdspath = c.write_gds(flatten_invalid_refs=True)
+    # gf.show(gdspath)
     c.show()
 
     # c1.write_gds("a.gds")
 
     # c2 = gf.read.import_gds("a.gds")
     # c2 = c2.flatten()
```

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.96.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzit.py` & `gdsfactory-6.96.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.96.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/mzm.py` & `gdsfactory-6.96.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/nxn.py` & `gdsfactory-6.96.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.96.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.96.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/optimal_step.py` & `gdsfactory-6.96.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/pack_doe.py` & `gdsfactory-6.96.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/pad.py` & `gdsfactory-6.96.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.96.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.96.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.96.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ramp.py` & `gdsfactory-6.96.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/rectangle.py` & `gdsfactory-6.96.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.96.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.96.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.96.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.96.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring.py` & `gdsfactory-6.96.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_crow.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_double.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.96.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/seal_ring.py` & `gdsfactory-6.96.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/snspd.py` & `gdsfactory-6.96.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/spiral_double.py` & `gdsfactory-6.96.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.96.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.96.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.96.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.96.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.96.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight.py` & `gdsfactory-6.96.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_array.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_pin.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/straight_rib.py` & `gdsfactory-6.96.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/switch_tree.py` & `gdsfactory-6.96.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/taper.py` & `gdsfactory-6.96.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.96.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.96.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.96.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.96.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/terminator.py` & `gdsfactory-6.96.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/text.py` & `gdsfactory-6.96.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/text_freetype.py` & `gdsfactory-6.96.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.96.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.96.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/triangles.py` & `gdsfactory-6.96.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/verniers.py` & `gdsfactory-6.96.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/version_stamp.py` & `gdsfactory-6.96.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via.py` & `gdsfactory-6.96.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via_corner.py` & `gdsfactory-6.96.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via_cutback.py` & `gdsfactory-6.96.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via_stack.py` & `gdsfactory-6.96.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.96.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.96.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/wafer.py` & `gdsfactory-6.96.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/wire.py` & `gdsfactory-6.96.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.96.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/config.py` & `gdsfactory-6.96.0/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.95.0"
+__version__ = "6.96.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-6.95.0/gdsfactory/constants.py` & `gdsfactory-6.96.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/containers.py` & `gdsfactory-6.96.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/cross_section.py` & `gdsfactory-6.96.0/gdsfactory/cross_section.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,17 +480,17 @@
     )
 
 
 radius_nitride = 20
 radius_rib = 20
 
 
-strip = cross_section
+# strip = cross_section
 strip_pins = partial(cross_section, add_pins=add_pins_inside1nm, name="strip")
-# strip = strip_pins
+strip = strip_pins
 strip_auto_widen = partial(strip, width_wide=0.9, auto_widen=True)
 strip_no_pins = partial(
     strip, add_pins=None, add_bbox=None, cladding_layers=None, cladding_offsets=None
 )
 strip_siepic = partial(cross_section, add_pins=add_pins_siepic_optical)
 
 # Rib with rectangular slab
```

### Comparing `gdsfactory-6.95.0/gdsfactory/decorators.py` & `gdsfactory-6.96.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/difftest.py` & `gdsfactory-6.96.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/events.py` & `gdsfactory-6.96.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/export/to_3d.py` & `gdsfactory-6.96.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/export/to_np.py` & `gdsfactory-6.96.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/export/to_stl.py` & `gdsfactory-6.96.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/export/write_gerbers.py` & `gdsfactory-6.96.0/gdsfactory/export/write_gerbers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/filestorage.py` & `gdsfactory-6.96.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/fill.py` & `gdsfactory-6.96.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/font.py` & `gdsfactory-6.96.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/functions.py` & `gdsfactory-6.96.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.96.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.96.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.96.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.96.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/README.md` & `gdsfactory-6.96.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.95.0</version>
+  <version>6.96.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 0% similar despite different names*

#### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.95.0&quot;
+__version__ = &quot;6.96.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.96.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.96.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/__init__.py` & `gdsfactory-6.96.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/boolean.py` & `gdsfactory-6.96.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.96.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.96.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.96.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.96.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.96.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/check_space.py` & `gdsfactory-6.96.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/check_width.py` & `gdsfactory-6.96.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.96.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.96.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/fillet.py` & `gdsfactory-6.96.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/functions.py` & `gdsfactory-6.96.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/invert.py` & `gdsfactory-6.96.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.96.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.96.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.96.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.96.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/offset.py` & `gdsfactory-6.96.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/outline.py` & `gdsfactory-6.96.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/trim.py` & `gdsfactory-6.96.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/union.py` & `gdsfactory-6.96.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-6.96.0/gdsfactory/geometry/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.96.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.96.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/get_factories.py` & `gdsfactory-6.96.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/get_netlist.py` & `gdsfactory-6.96.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.96.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.96.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/grid.py` & `gdsfactory-6.96.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/install.py` & `gdsfactory-6.96.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/klive.py` & `gdsfactory-6.96.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/__init__.py` & `gdsfactory-6.96.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.96.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/ehva.py` & `gdsfactory-6.96.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.96.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/siepic.py` & `gdsfactory-6.96.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/labels/write_labels.py` & `gdsfactory-6.96.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/materials.py` & `gdsfactory-6.96.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/name.py` & `gdsfactory-6.96.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/pack.py` & `gdsfactory-6.96.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/path.py` & `gdsfactory-6.96.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/pdk.py` & `gdsfactory-6.96.0/gdsfactory/pdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         default="warn",
         description="""Action to take when a duplicate cell is encountered on gds write (usually problematic). Options are
                         "warn" (default): overwrite all duplicate cells with one of the duplicates (arbitrarily).
                         "error": throw a ValueError when attempting to write a gds with duplicate cells.
                         "overwrite": overwrite all duplicate cells with one of the duplicates, without warning.""",
     )
     flatten_invalid_refs: bool = Field(
-        default=False,
+        default=True,
         description="If true, will auto-correct (and flatten) cell references which are off-grid or rotated by non-manhattan angles.",
     )
     max_points: int = Field(
         default=4000,
         description="Maximum number of points to allow in a polygon before fracturing.",
     )
```

### Comparing `gdsfactory-6.95.0/gdsfactory/picmodel.py` & `gdsfactory-6.96.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/pixelate.py` & `gdsfactory-6.96.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.96.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/database/README.md` & `gdsfactory-6.96.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.96.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/database/models.py` & `gdsfactory-6.96.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/web/main.py` & `gdsfactory-6.96.0/gdsfactory/plugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/web/server.py` & `gdsfactory-6.96.0/gdsfactory/plugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/web/server_jupyter.py` & `gdsfactory-6.96.0/gdsfactory/plugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/plugins/web/static/client.css` & `gdsfactory-6.96.0/gdsfactory/plugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/port.py` & `gdsfactory-6.96.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/quickplotter.py` & `gdsfactory-6.96.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/__init__.py` & `gdsfactory-6.96.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_dphox.py` & `gdsfactory-6.96.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.96.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_np.py` & `gdsfactory-6.96.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_phidl.py` & `gdsfactory-6.96.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_yaml.py` & `gdsfactory-6.96.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.96.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/import_gds.py` & `gdsfactory-6.96.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/read/labels.py` & `gdsfactory-6.96.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/__init__.py` & `gdsfactory-6.96.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/add_pads.py` & `gdsfactory-6.96.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/all_angle.py` & `gdsfactory-6.96.0/gdsfactory/routing/all_angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 def _get_bend_ports(bend):
     # this is a bit of a hack, but o1 < o2, in0 < out0, hopefully there are no other wacky conventions!
     sorted_port_names = sorted(bend.ports.keys())
     return [bend.ports[n] for n in sorted_port_names]
 
 
 LOW_LOSS_CROSS_SECTIONS = [
-    {"cross_section": "strip", "settings": {"width": 1.0}},
+    {"cross_section": "strip", "settings": {"width": 0.9}},
     "strip",
 ]
 
 
 def low_loss_connector(
     port1: Port,
     port2: Port,
```

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.96.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/factories.py` & `gdsfactory-6.96.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/fanout.py` & `gdsfactory-6.96.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.96.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_route.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.96.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/manhattan.py` & `gdsfactory-6.96.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.96.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_quad.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/route_south.py` & `gdsfactory-6.96.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.96.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/routing/utils.py` & `gdsfactory-6.96.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.96.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/03_move.py` & `gdsfactory-6.96.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/04_connect.py` & `gdsfactory-6.96.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.96.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.96.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.96.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.96.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.96.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.96.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-6.96.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.96.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.96.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/17_ports.py` & `gdsfactory-6.96.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/20_components.py` & `gdsfactory-6.96.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.96.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.96.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.96.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.96.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.96.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.96.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.96.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.96.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/big_device.py` & `gdsfactory-6.96.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.96.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.96.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.96.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: bend_euler_f84cb6d2
+name: bend_euler_af89db80
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -35,14 +35,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
   child: null
   default:
     angle: 90.0
     cross_section: strip
     direction: ccw
     npoints: null
@@ -60,14 +61,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     direction: ccw
     npoints: null
     p: 0.5
     with_arc_floorplan: true
     with_bbox: true
   function_name: bend_euler
@@ -108,8 +110,8 @@
       start_straight_length: 0.01
       taper_length: 10.0
       width: 0.5
       width_wide: null
     width: 1.0
   info_version: 2
   module: gdsfactory.components.bend_euler
-  name: bend_euler_f84cb6d2
+  name: bend_euler_af89db80
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: grating_coupler_ellipti_514a8b8c
+name: grating_coupler_ellipti_9a60b03b
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -35,14 +35,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     grating_line_width: 0.6
     layer_slab: null
   child: null
   default:
     big_last_tooth: false
     cross_section: strip
@@ -70,14 +71,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     fiber_angle: 15.0
     grating_line_width: 0.6
     layer_slab: null
     n_periods: 30
     nclad: 1.443
     neff: 2.638
@@ -90,8 +92,8 @@
     wavelength: 1.554
   function_name: grating_coupler_elliptical
   info:
     polarization: te
     wavelength: 1.554
   info_version: 2
   module: gdsfactory.components.grating_coupler_elliptical
-  name: grating_coupler_ellipti_514a8b8c
+  name: grating_coupler_ellipti_9a60b03b
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-name: mmi1x2_1fb8ba6f
+name: mmi1x2_fc7db243
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
     - 0
     name: o1
     orientation: 180
     port_type: optical
     shear_angle: null
-    width: 1.0
+    width: 0.9
   o2:
     center:
     - 15.5
     - 0.625
     layer:
     - 34
     - 0
     name: o2
     orientation: 0.0
     port_type: optical
     shear_angle: null
-    width: 1.0
+    width: 0.9
   o3:
     center:
     - 15.5
     - -0.625
     layer:
     - 34
     - 0
     name: o3
     orientation: 0.0
     port_type: optical
     shear_angle: null
-    width: 1.0
+    width: 0.9
 settings:
   changed:
     cross_section:
       function: cross_section
       settings:
         add_pins:
           function: add_pins
@@ -47,17 +47,17 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
-        width: 1.0
-    width: 1.0
-    width_mmi: 3
+        name: strip
+        width: 0.9
+    width: 0.9
   child: null
   default:
     cross_section: strip
     gap_mmi: 0.25
     length_mmi: 5.5
     length_taper: 10.0
     taper:
@@ -76,22 +76,23 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
-        width: 1.0
+        name: strip
+        width: 0.9
     gap_mmi: 0.25
     length_mmi: 5.5
     length_taper: 10.0
     taper:
       function: taper
-    width: 1.0
-    width_mmi: 3
+    width: 0.9
+    width_mmi: 2.5
     width_taper: 1.0
     with_bbox: true
   function_name: mmi1x2
   info: {}
   info_version: 2
   module: gdsfactory.components.mmi1x2
-  name: mmi1x2_1fb8ba6f
+  name: mmi1x2_fc7db243
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-name: mmi1x2_77b0da92
+name: mmi1x2_b84370c5
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
     - 0
     name: o1
     orientation: 180
     port_type: optical
     shear_angle: null
-    width: 0.9
+    width: 1.0
   o2:
     center:
     - 15.5
     - 0.625
     layer:
     - 34
     - 0
     name: o2
     orientation: 0.0
     port_type: optical
     shear_angle: null
-    width: 0.9
+    width: 1.0
   o3:
     center:
     - 15.5
     - -0.625
     layer:
     - 34
     - 0
     name: o3
     orientation: 0.0
     port_type: optical
     shear_angle: null
-    width: 0.9
+    width: 1.0
 settings:
   changed:
     cross_section:
       function: cross_section
       settings:
         add_pins:
           function: add_pins
@@ -47,16 +47,18 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
-        width: 0.9
-    width: 0.9
+        name: strip
+        width: 1.0
+    width: 1.0
+    width_mmi: 3
   child: null
   default:
     cross_section: strip
     gap_mmi: 0.25
     length_mmi: 5.5
     length_taper: 10.0
     taper:
@@ -75,22 +77,23 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
-        width: 0.9
+        name: strip
+        width: 1.0
     gap_mmi: 0.25
     length_mmi: 5.5
     length_taper: 10.0
     taper:
       function: taper
-    width: 0.9
-    width_mmi: 2.5
+    width: 1.0
+    width_mmi: 3
     width_taper: 1.0
     with_bbox: true
   function_name: mmi1x2
   info: {}
   info_version: 2
   module: gdsfactory.components.mmi1x2
-  name: mmi1x2_77b0da92
+  name: mmi1x2_b84370c5
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: mzi_e687e91e
+name: mzi_6cace905
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
@@ -38,14 +38,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         with_bbox: true
     cross_section:
       function: cross_section
       settings:
         add_pins:
           function: add_pins
@@ -53,14 +54,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     splitter:
       function: mmi1x2
       settings:
         cross_section:
           function: cross_section
           settings:
@@ -70,14 +72,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         width: 1.0
         width_mmi: 3
     straight:
       function: straight
       settings:
         cross_section:
@@ -89,14 +92,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         with_bbox: true
   child: null
   default:
     add_optical_ports_arms: false
     bend:
       function: bend_euler
@@ -134,14 +138,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         with_bbox: true
     combiner: null
     cross_section:
       function: cross_section
       settings:
         add_pins:
@@ -150,14 +155,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     cross_section_x_bot: null
     cross_section_x_top: null
     delta_length: 10.0
     length_x: 0.1
     length_y: 2.0
     mirror_bot: false
@@ -178,14 +184,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         width: 1.0
         width_mmi: 3
     straight:
       function: straight
       settings:
         cross_section:
@@ -197,18 +204,19 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 1.0
         with_bbox: true
     straight_x_bot: null
     straight_x_top: null
     straight_y: null
     with_splitter: true
   function_name: mzi
   info: {}
   info_version: 2
   module: gdsfactory.components.mzi
-  name: mzi_e687e91e
+  name: mzi_6cace905
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: mzi_f7f1cb39
+name: mzi_435017ce
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
@@ -38,14 +38,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         with_bbox: true
     cross_section:
       function: cross_section
       settings:
         add_pins:
           function: add_pins
@@ -53,14 +54,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 0.9
     splitter:
       function: mmi1x2
       settings:
         cross_section:
           function: cross_section
           settings:
@@ -70,14 +72,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         width: 0.9
     straight:
       function: straight
       settings:
         cross_section:
           function: cross_section
@@ -88,14 +91,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         with_bbox: true
   child: null
   default:
     add_optical_ports_arms: false
     bend:
       function: bend_euler
@@ -133,14 +137,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         with_bbox: true
     combiner: null
     cross_section:
       function: cross_section
       settings:
         add_pins:
@@ -149,14 +154,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 0.9
     cross_section_x_bot: null
     cross_section_x_top: null
     delta_length: 10.0
     length_x: 0.1
     length_y: 2.0
     mirror_bot: false
@@ -177,14 +183,15 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         width: 0.9
     straight:
       function: straight
       settings:
         cross_section:
           function: cross_section
@@ -195,18 +202,19 @@
             - - 36
               - 0
             bbox_offsets:
             - 3
             layer:
             - 34
             - 0
+            name: strip
             width: 0.9
         with_bbox: true
     straight_x_bot: null
     straight_x_top: null
     straight_y: null
     with_splitter: true
   function_name: mzi
   info: {}
   info_version: 2
   module: gdsfactory.components.mzi
-  name: mzi_f7f1cb39
+  name: mzi_435017ce
```

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.96.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: straight_f84cb6d2
+name: straight_af89db80
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -35,14 +35,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
   child: null
   default:
     cross_section: strip
     length: 10.0
     npoints: 2
     with_bbox: true
@@ -56,14 +57,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     length: 10.0
     npoints: 2
     with_bbox: true
   function_name: straight
   info:
     cross_section:
@@ -75,14 +77,15 @@
         - - 36
           - 0
         bbox_offsets:
         - 3
         layer:
         - 34
         - 0
+        name: strip
         width: 1.0
     function_name: cross_section
     length: 10.0
     settings:
       add_bbox: null
       add_pins: null
       auto_widen: false
@@ -113,8 +116,8 @@
       start_straight_length: 0.01
       taper_length: 10.0
       width: 0.5
       width_wide: null
     width: 1.0
   info_version: 2
   module: gdsfactory.components.straight
-  name: straight_f84cb6d2
+  name: straight_af89db80
```

### Comparing `gdsfactory-6.95.0/gdsfactory/schematic_editor.py` & `gdsfactory-6.96.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/serialization.py` & `gdsfactory-6.96.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/show.py` & `gdsfactory-6.96.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.96.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.96.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.96.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.96.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.96.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.96.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.96.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.96.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.96.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/modes.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,15 +512,15 @@
             )
 
         return self._waveguide
 
     def coupling_length(self, power_ratio: float = 1.0) -> float:
         """Coupling length calculated from the effective mode indices.
 
-        Parameters:
+        Args:
             power_ratio: desired coupling power ratio.
         """
         m = (self.n_eff.size // 2) * 2
         n_even = self.n_eff[:m:2].real
         n_odd = self.n_eff[1:m:2].real
         return (
             self.wavelength / (np.pi * (n_even - n_odd)) * np.arcsin(power_ratio**0.5)
@@ -570,15 +570,15 @@
 
 def sweep_n_eff(waveguide: Waveguide, **sweep_kwargs) -> np.ndarray:
     """Return the effective index for a range of waveguide geometries.
 
     The returned array uses the sweep arguments and the mode index as
     coordinates to organize the data.
 
-    Parameters:
+    Args:
         waveguide: base waveguide geometry.
         sweep_kwargs: Waveguide arguments and values to sweep.
 
     Example:
         >>> sweep_n_eff(
         ...     my_waveguide,
         ...     core_width=[0.40, 0.45, 0.50],
@@ -590,15 +590,15 @@
 
 def sweep_n_group(waveguide: Waveguide, **sweep_kwargs) -> np.ndarray:
     """Return the group index for a range of waveguide geometries.
 
     The returned array uses the sweep arguments and the mode index as
     coordinates to organize the data.
 
-    Parameters:
+    Args:
         waveguide: base waveguide geometry.
         sweep_kwargs: Waveguide arguments and values to sweep.
 
     Example:
         >>> sweep_n_group(
         ...     my_waveguide,
         ...     core_width=[0.40, 0.45, 0.50],
@@ -610,15 +610,15 @@
 
 def sweep_mode_area(waveguide: Waveguide, **sweep_kwargs) -> np.ndarray:
     """Return the mode area for a range of waveguide geometries.
 
     The returned array uses the sweep arguments and the mode index as
     coordinates to organize the data.
 
-    Parameters:
+    Args:
         waveguide: base waveguide geometry.
         sweep_kwargs: Waveguide arguments and values to sweep.
 
     Example:
         >>> sweep_mode_area(
         ...     my_waveguide,
         ...     core_width=[0.40, 0.45, 0.50],
@@ -632,15 +632,15 @@
     waveguide: Waveguide, bend_radii: Tuple[float, ...]
 ) -> np.ndarray:
     """Overlap integral squared for the bend mode mismatch loss.
 
     The loss is squared because you hit the bend loss twice
     (from bend to straight and from straight to bend).
 
-    Parameters:
+    Args:
         waveguide: base waveguide geometry.
         bend_radii: radii values to sweep.
     """
     kwargs = dict(waveguide)
     kwargs.pop("bend_radius")
     straight = Waveguide(**kwargs)
```

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.96.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.96.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.96.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/plot.py` & `gdsfactory-6.96.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.96.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.96.0/gdsfactory/simulation/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.96.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.96.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.96.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.96.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.96.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.96.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.96.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.96.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/snap.py` & `gdsfactory-6.96.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/symbols.py` & `gdsfactory-6.96.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/__init__.py` & `gdsfactory-6.96.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.96.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/layer_map.py` & `gdsfactory-6.96.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.96.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/layer_views.py` & `gdsfactory-6.96.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.96.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/types.py` & `gdsfactory-6.96.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/typings.py` & `gdsfactory-6.96.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/utils/async_utils.py` & `gdsfactory-6.96.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/utils/file_utils.py` & `gdsfactory-6.96.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.96.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.96.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/watch.py` & `gdsfactory-6.96.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.96.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/gdsfactory/write_cells.py` & `gdsfactory-6.96.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.95.0/pyproject.toml` & `gdsfactory-6.96.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
-version = "6.95.0"
+version = "6.96.0"
 authors = [
 {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 dependencies = [
   "click",
```

### Comparing `gdsfactory-6.95.0/PKG-INFO` & `gdsfactory-6.96.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.95.0
+Version: 6.96.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -114,15 +114,15 @@
 Provides-Extra: full
 Provides-Extra: gmsh
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.95.0
+# gdsfactory 6.96.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

