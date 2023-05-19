# Comparing `tmp/peegy-1.4.3.tar.gz` & `tmp/peegy-1.4.4.tar.gz`

## Comparing `peegy-1.4.3.tar` & `peegy-1.4.4.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitattributes
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.4.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.4.3/MANIFEST.in
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 peegy-1.4.3/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 peegy-1.4.3/requirements.txt
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.4.3/setup.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/README.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/__init__.py
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_abr_peak_detection.py
--rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_eog_removal_template_.py
--rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection_bootstrap.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection_filters.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_video.py
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_weighted_average.py
--rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_weighted_vs_standard_average.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_dss_time_domain_bias_test.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_f_test.py
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test.py
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test_weighted_average.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_no_layout.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_phase_locking_value_test.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_ffr_artifact_removal.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_using_own_data_trials.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_using_own_raw_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/channel_definitions.py
--rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/edf_bdf_reader.py
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/eegReaderAbstractClasses.py
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/eeg_definitions.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/events.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/directories/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/directories/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/__init__.py
--rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/edf_bdf_reader.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/generic_csv_reader.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/synergy_reader.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/xml_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/eeg/__init__.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/eeg/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/__init__.py
--rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/file_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/__init__.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/__init__.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/data_storage_reading_tools.py
--rw-r--r--   0        0        0    16923 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/data_storage_tools.py
--rw-r--r--   0        0        0    29698 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/plot_tools.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/KIT-160.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi128.lay
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi16.lay
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi160.lay
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi256.lay
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32.lay
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_2_EXT.lay
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64.lay
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64_2_EXT.lay
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64_3_EXT.lay
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/emotive14.lay
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/layouts.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/neuroscan64.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/__init__.py
--rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/eeg_plot_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/events/__init__.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/events/event_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/__init__.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/attach.py
--rw-r--r--   0        0        0    27695 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/definitions.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/detection.py
--rw-r--r--   0        0        0    31500 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/epochs.py
--rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/general.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/interpolation.py
--rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/io.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/pipeline.py
--rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/plot.py
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/regression.py
--rw-r--r--   0        0        0    22084 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/simulate.py
--rw-r--r--   0        0        0    38597 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/spatial_filtering.py
--rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/statistics.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/storage.py
--rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/time_frequency.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/bootstrap/__init__.py
--rw-r--r--   0        0        0    22128 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/bootstrap/bootstrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/__init__.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/definitions.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/eeg_statistic_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/memory.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/progress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/__init__.py
--rw-r--r--   0        0        0    20462 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/eeg_epoch_operators.py
--rw-r--r--   0        0        0    69736 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/epochs_processing_tools.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/math_tools.py
--rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/weightedAverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/__init__.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/definitions.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/time_domain_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/__init__.py
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eegFiltering.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/resampling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eog_tools/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/fitting/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/fitting/fitting_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/multiprocessing/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/__init__.py
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/h0.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/video/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/video/recording.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/dss_unit_tests.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/eeg_test_resampling.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/javerager_test.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/read_data_test.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_assr_moving_average.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_average_spectrogram_power.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_biosemi_class.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_biosemi_reader.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_bootstraping.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_edf_reader.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eeg_notch_filter.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_removal_correlation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_template_removal.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_template_valderrama_20118.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_et_tools.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_filter.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fir_filter_mt.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fir_filter_ols.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fiter_mt.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_freq_noise_estimation.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_freq_noise_estimation_plots.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_frequency_average_epochs.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_generic_reader.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_hotelling_t2.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_ica_average_epochs.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_multiprocessing.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_noise_generator.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_norm_corr.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_parse_processing_chain.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_peakdetection.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_phase_locking_value.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_pooled_freq_noise_estimation.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_scrolling.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_example1.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_example6.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_w_average_epochs.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_xml_to_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/__init__.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/ir_test.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/aep_gui/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/signal_generator/__init__.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/signal_generator/noise_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/units/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/units/unit_tools.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitignore
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.4.3/LICENSE.txt
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 peegy-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 peegy-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitattributes
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.4.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.4.4/MANIFEST.in
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 peegy-1.4.4/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 peegy-1.4.4/requirements.txt
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.4.4/setup.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/__init__.py
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_abr_peak_detection.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_eog_removal_template_.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection_bootstrap.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection_filters.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_video.py
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_weighted_average.py
+-rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_weighted_vs_standard_average.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_dss_time_domain_bias_test.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_f_test.py
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test.py
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test_weighted_average.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_no_layout.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_phase_locking_value_test.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_ffr_artifact_removal.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_using_own_data_trials.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_using_own_raw_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/channel_definitions.py
+-rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/edf_bdf_reader.py
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/eegReaderAbstractClasses.py
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/eeg_definitions.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/events.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/directories/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/directories/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/__init__.py
+-rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/edf_bdf_reader.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/generic_csv_reader.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/synergy_reader.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/xml_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/eeg/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/eeg/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/__init__.py
+-rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/file_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/__init__.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/data_storage_reading_tools.py
+-rw-r--r--   0        0        0    16923 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/data_storage_tools.py
+-rw-r--r--   0        0        0    29698 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/plot_tools.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/KIT-160.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi128.lay
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi16.lay
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi160.lay
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi256.lay
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32.lay
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_2_EXT.lay
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64.lay
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64_2_EXT.lay
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64_3_EXT.lay
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/emotive14.lay
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/layouts.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/neuroscan64.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/__init__.py
+-rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/eeg_plot_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/events/__init__.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/events/event_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/attach.py
+-rw-r--r--   0        0        0    27695 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/definitions.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/detection.py
+-rw-r--r--   0        0        0    31702 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/epochs.py
+-rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/general.py
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/interpolation.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/io.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/pipeline.py
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/plot.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/regression.py
+-rw-r--r--   0        0        0    22127 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/simulate.py
+-rw-r--r--   0        0        0    38922 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/spatial_filtering.py
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/statistics.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/storage.py
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/time_frequency.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/bootstrap/__init__.py
+-rw-r--r--   0        0        0    22270 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/definitions.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/eeg_statistic_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/memory.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/progress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/__init__.py
+-rw-r--r--   0        0        0    21075 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/eeg_epoch_operators.py
+-rw-r--r--   0        0        0    70505 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/epochs_processing_tools.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/math_tools.py
+-rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/weightedAverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/__init__.py
+-rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/definitions.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/time_domain_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/__init__.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eegFiltering.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/resampling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/fitting/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/fitting/fitting_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/multiprocessing/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/__init__.py
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/h0.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/video/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/video/recording.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/dss_unit_tests.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/eeg_test_resampling.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/javerager_test.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/read_data_test.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_assr_moving_average.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_average_spectrogram_power.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_biosemi_class.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_biosemi_reader.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_bootstraping.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_edf_reader.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eeg_notch_filter.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_removal_correlation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_template_removal.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_template_valderrama_20118.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_et_tools.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_filter.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fir_filter_mt.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fir_filter_ols.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fiter_mt.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_freq_noise_estimation.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_freq_noise_estimation_plots.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_frequency_average_epochs.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_generic_reader.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_hotelling_t2.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_ica_average_epochs.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_multiprocessing.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_noise_generator.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_norm_corr.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_parse_processing_chain.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_peakdetection.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_phase_locking_value.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_scrolling.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_example1.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_example6.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_w_average_epochs.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_xml_to_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/__init__.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/ir_test.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/signal_generator/__init__.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/signal_generator/noise_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/units/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/units/unit_tools.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 peegy-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 peegy-1.4.4/PKG-INFO
```

### Comparing `peegy-1.4.3/.gitlab-ci.yml` & `peegy-1.4.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/CODE_OF_CONDUCT.md` & `peegy-1.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/CONTRIBUTING.md` & `peegy-1.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/Readme.md` & `peegy-1.4.4/Readme.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/requirements.txt` & `peegy-1.4.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/setup.py` & `peegy-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_abr_peak_detection.py` & `peegy-1.4.4/examples/example_abr_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_eog_removal_template_.py` & `peegy-1.4.4/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_peak_detection.py` & `peegy-1.4.4/examples/example_acc_peak_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                            mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
                            layout_file_name='biosemi32.lay',
                            snr=0.1,
                            event_times=event_times,
                            event_code=1.0,
                            figures_subset_folder='acc_test',
                            include_eog_events=True,
+                           noise_attenuation=0,
                            )
 reader.run()
 
 # %%
 # Start the pipeline
 # ============================
 # Now we proceed with our basic processing pipeline
```

### Comparing `peegy-1.4.3/examples/example_acc_peak_detection_bootstrap.py` & `peegy-1.4.4/examples/example_acc_peak_detection_bootstrap.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_peak_detection_filters.py` & `peegy-1.4.4/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_video.py` & `peegy-1.4.4/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_weighted_average.py` & `peegy-1.4.4/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.4.4/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.4.4/examples/example_assr_dss_frequency_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.4.4/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_f_test.py` & `peegy-1.4.4/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_ht2_test.py` & `peegy-1.4.4/examples/example_assr_ht2_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.4.4/examples/example_assr_ht2_test_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.4.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_no_layout.py` & `peegy-1.4.4/examples/example_assr_no_layout.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_assr_phase_locking_value_test.py` & `peegy-1.4.4/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_ffr_artifact_removal.py` & `peegy-1.4.4/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_using_own_data_trials.py` & `peegy-1.4.4/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/examples/example_using_own_raw_data.py` & `peegy-1.4.4/examples/example_using_own_raw_data.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/channel_definitions.py` & `peegy-1.4.4/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/edf_bdf_reader.py` & `peegy-1.4.4/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.4.4/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/eeg_definitions.py` & `peegy-1.4.4/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/events.py` & `peegy-1.4.4/peegy/definitions/events.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/definitions/tables.py` & `peegy-1.4.4/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/directories/tools.py` & `peegy-1.4.4/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/edf_bdf_reader.py` & `peegy-1.4.4/peegy/io/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/generic_csv_reader.py` & `peegy-1.4.4/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/synergy_reader.py` & `peegy-1.4.4/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/xml_tools.py` & `peegy-1.4.4/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/eeg/reader.py` & `peegy-1.4.4/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/external_tools/file_tools.py` & `peegy-1.4.4/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.4.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.4.4/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.4.4/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.4.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.4.4/peegy/io/storage/data_storage_reading_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/storage/data_storage_tools.py` & `peegy-1.4.4/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/io/storage/plot_tools.py` & `peegy-1.4.4/peegy/io/storage/plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/KIT-160.lay` & `peegy-1.4.4/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi128.lay` & `peegy-1.4.4/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi16.lay` & `peegy-1.4.4/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi160.lay` & `peegy-1.4.4/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi256.lay` & `peegy-1.4.4/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi32.lay` & `peegy-1.4.4/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.4.4/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.4.4/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.4.4/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi64.lay` & `peegy-1.4.4/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.4.4/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.4.4/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/emotive14.lay` & `peegy-1.4.4/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/layouts.py` & `peegy-1.4.4/peegy/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/layouts/neuroscan64.lay` & `peegy-1.4.4/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.4.4/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/plot/eeg_plot_tools.py` & `peegy-1.4.4/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/events/event_tools.py` & `peegy-1.4.4/peegy/processing/events/event_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/attach.py` & `peegy-1.4.4/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/definitions.py` & `peegy-1.4.4/peegy/processing/pipe/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/detection.py` & `peegy-1.4.4/peegy/processing/pipe/detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/epochs.py` & `peegy-1.4.4/peegy/processing/pipe/epochs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from peegy.definitions.tables import Tables
 from peegy.processing.statistics.eeg_statistic_tools import hotelling_t_square_test, f_test
 from peegy.processing.tools.eeg_epoch_operators import w_mean, effective_sampling_size
 import numpy as np
 import pandas as pd
 import os
 import pyfftw
-import multiprocessing
 import astropy.units as u
 from tqdm import tqdm
 from peegy.tools.units.unit_tools import set_default_unit
 from PyQt5.QtCore import QLibraryInfo
 os.environ["QT_QPA_PLATFORM_PLUGIN_PATH"] = QLibraryInfo.location(QLibraryInfo.PluginsPath)
 
 
@@ -394,14 +393,15 @@
                  n_fft: int = None,
                  weighted_average: bool = True,
                  weighted_frequency_domain: bool = False,
                  weight_across_epochs: bool = True,
                  weight_frequencies: np.array = None,
                  delta_frequency: u.Quantity = 5. * u.Hz,
                  power_line_frequency: u.Quantity = 50 * u.Hz,
+                 n_jobs: int = 1,
                  **kwargs):
         """
         This InputOutputProcess average epochs in the frequency domain
         :param input_process: InputOutputProcess Class
         :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         :param block_size: number of trials that will be stack together to estimate the residual noise
         :param test_frequencies: numpy array with frequencies that will be used to compute statistics (Hotelling test)
@@ -410,26 +410,28 @@
         :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
         are computed within epoch (1 / variance across time)
         :param weight_frequencies: numpy array with frequencies that will be used to estimate weights when
         weighted_average is activated
         :param delta_frequency: frequency size around each test_frequencies to estimate weights and noise
         :param power_line_frequency: frequency of local power line frequency. This will be used to prevent using
         this frequency or its multiples when performing frequency statistics
+        :param n_jobs: number of CPUs to compute fft
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(AverageEpochsFrequencyDomain, self).__init__(input_process=input_process, **kwargs)
         self.n_tracked_points = n_tracked_points
         self.block_size = block_size
         self.test_frequencies = set_default_unit(test_frequencies, u.Hz)
         self.weight_frequencies = set_default_unit(weight_frequencies, u.Hz)
         self.weighted_average = weighted_average
         self.weighted_frequency_domain = weighted_frequency_domain
         self.weight_across_epochs = weight_across_epochs
         self.delta_frequency = set_default_unit(delta_frequency, u.Hz)
         self.power_line_frequency = set_default_unit(power_line_frequency, u.Hz)
+        self.n_jobs = n_jobs
 
     def transform_data(self):
         # average processed data across epochs including frequency average
         if self.weighted_frequency_domain:
             if self.weight_frequencies is None and self.test_frequencies is not None:
                 print('No specific frequency provided to estimate weights in the frequency-domain. Pooling across '
                       'test frequencies {:}. Results may be inaccurate if test frequencies contain no '
@@ -442,15 +444,16 @@
             w_ave, snr, rn, by_freq_rn, by_freq_snr, w_fft, w, freq_samples, exact_frequencies = et_frequency_mean2(
                 epochs=self.input_node.data,
                 fs=self.input_node.fs,
                 weighted_average=self.weighted_average,
                 test_frequencies=self.test_frequencies,
                 delta_frequency=self.delta_frequency,
                 block_size=self.block_size,
-                power_line_frequency=self.power_line_frequency
+                power_line_frequency=self.power_line_frequency,
+                n_jobs=self.n_jobs
             )
         else:
             if self.n_tracked_points is None:
                 self.n_tracked_points = self.input_node.data.shape[0]
             samples_distance = int(max(self.input_node.data.shape[0] // self.n_tracked_points, 1))
             w_ave, w, rn, cum_rn, w_fft, n, wb, nb, snr = \
                 et_mean(epochs=self.input_node.data,
@@ -462,19 +465,22 @@
             if self.test_frequencies is not None:
                 n = w_ave.shape[0]
                 freqs = np.arange(0, n) * self.input_node.fs / n
                 k = np.array([np.argmin(np.abs(freqs - _f)) for _f in self.test_frequencies])
                 exact_frequencies = freqs[k]
 
             if exact_frequencies.size:
-                _fft = pyfftw.builders.rfft(self.input_node.data, overwrite_input=False, planner_effort='FFTW_ESTIMATE',
+                _fft = pyfftw.builders.rfft(self.input_node.data,
+                                            overwrite_input=False,
+                                            planner_effort='FFTW_ESTIMATE',
                                             axis=0,
-                                            threads=multiprocessing.cpu_count())
+                                            threads=self.n_jobs)()
+
                 scaling_factor = 2 / self.input_node.data.shape[0]
-                _fft_samples = _fft() * scaling_factor * self.input_node.data.unit
+                _fft_samples = _fft * scaling_factor * self.input_node.data.unit
                 freq_samples = _fft_samples[k, ...]
 
         hts = []
         for _idx, _f in enumerate(exact_frequencies):
             _freq_samples = freq_samples[_idx, :, :]
             h_samples = np.vstack((np.real(_freq_samples), np.imag(_freq_samples)))
             h_samples = h_samples.reshape((2, *freq_samples.shape[1::]))
```

### Comparing `peegy-1.4.3/peegy/processing/pipe/general.py` & `peegy-1.4.4/peegy/processing/pipe/general.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/interpolation.py` & `peegy-1.4.4/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/io.py` & `peegy-1.4.4/peegy/processing/pipe/io.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/pipeline.py` & `peegy-1.4.4/peegy/processing/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/plot.py` & `peegy-1.4.4/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/regression.py` & `peegy-1.4.4/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/simulate.py` & `peegy-1.4.4/peegy/processing/pipe/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,15 @@
         for _i, _ne in enumerate(_new_noise_events):
             _ini_pos = int(_ne * fs)
             _noise_samples = np.random.randint(1, int(fs * noise_events_duration))
             _ini_pos = np.minimum(_ini_pos, size)
             _end_pos = np.minimum(_ini_pos + _noise_samples - 1, size)
             noise[_ini_pos:_end_pos, :] += np.random.normal(0, 10 ** (noise_events_power_delta_db / 20) * 0.1,
                                                             size=(_end_pos - _ini_pos, n_channels))
+    noise = noise - np.mean(noise, axis=0)
     return noise, stationary_noise_var
 
 
 def generate_line_noise(size: int = None,
                         fs: u.Quantity = None,
                         n_channels: int = None,
                         line_noise_mixing_matrix: np.array = None,
```

### Comparing `peegy-1.4.3/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.4.4/peegy/processing/pipe/spatial_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                  keep0: int = None,
                  keep1: float = 1e-9,
                  perc0: float = .99,
                  perc1: float = None,
                  block_size: int = 10,
                  n_tracked_points: int = None,
                  delta_frequency: u.Quantity = 5 * u.Hz,
+                 n_jobs: int = 1,
                  **kwargs):
         """
         This class will create a spatial filter based on the data. If sf_join_frequencies are passed, the spatial
         filter will use a biased function based on the covariance of those frequencies only.
         :param input_process:  InputOutputProcess Class
         :param sf_join_frequencies: numpy array indicating the biased frequencies (useful for steady-state responses)
         :param demean_data: if true, data will be demeaned prior filter estimation
@@ -52,14 +53,15 @@
         :param perc0: float (between 0 and 1) controlling whitening of unbiased components in DSS.
         This value will preserve components that explain the percentage of variance.
         :param perc1: float (between 0 and 1) controlling the number of biased components kept in DSS.
         This value will preserve the components of the biased PCA analysis that explain the percentage of variance.
         :param block_size: integer indicating the number of trials that would be used to estimate the weights
         :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         :param delta_frequency: frequency size around each sf_join_frequency to estimate noise
+        :param n_jobs: number of CPUs to compute FFT
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(SpatialFilter, self).__init__(input_process=input_process, **kwargs)
         self.sf_join_frequencies = set_default_unit(sf_join_frequencies, u.Hz)
         self.demean_data = demean_data
         self.weight_data = weight_data
         self.weighted_frequency_domain = weighted_frequency_domain
@@ -74,14 +76,15 @@
         self.keep1 = keep1
         self.perc0 = perc0
         self.perc1 = perc1
         self.block_size = block_size
         self.n_tracked_points = n_tracked_points
         self.delta_frequency = delta_frequency
         self.weights = None
+        self.n_jobs = n_jobs
 
     def transform_data(self):
         # compute spatial filter
         z, pwr0, pwr1, cov, n_0, n_1, weights = et_get_spatial_filtering(
             epochs=self.input_node.data,
             fs=self.input_node.fs,
             sf_join_frequencies=self.sf_join_frequencies,
@@ -92,15 +95,17 @@
             weights=self.input_node.w,
             keep0=self.keep0,
             keep1=self.keep1,
             perc0=self.perc0,
             perc1=self.perc1,
             block_size=self.block_size,
             n_tracked_points=self.n_tracked_points,
-            delta_frequency=self.delta_frequency)
+            delta_frequency=self.delta_frequency,
+            n_jobs=self.n_jobs
+        )
         self.output_node.data = z * u.dimensionless_unscaled
         self.pwr0 = pwr0
         self.pwr1 = pwr1
         self.cov = cov
         self.n_components_rotation_1 = n_0
         self.n_components_rotation_2 = n_1
         self.n_possible_components = self.input_node.data.shape[1]
@@ -161,14 +166,15 @@
                  plot_power: bool = True,
                  plot_x_lim: [float, float] = None,
                  plot_y_lim: [float, float] = None,
                  user_naming_rule: str = '',
                  fig_format: str = '.png',
                  return_figures: bool = False,
                  save_to_file: bool = True,
+                 n_jobs: int = 1,
                  **kwargs):
         """
         This class will create and apply a spatial filter to the data.
         :param input_process: an InputOutputProcess Class
         :param sf_join_frequencies: numpy array indicating the biased frequencies (useful for steady-state responses)
         :param sf_components: numpy array of integers with indexes of components to be kept
         :param sf_thr: float indicating the percentage of explained variance by components to be kept (this is used when
@@ -195,14 +201,15 @@
         :param user_naming_rule: string indicating a user naming to be included in the figure file name
         :param fig_format: string indicating the format of the output figure (e.g. '.png' or '.pdf')
         :param return_figures: bool indicating if figure handle should be returned in self.figures
         :param save_to_file: bool indicating whether figure should be saved to file
         :param block_size: number of trials that will be stacked together to estimate the residual noise
         :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         n_tracked_points
+        :param n_jobs: number of CPUs for fft
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(CreateAndApplySpatialFilter, self).__init__(input_process=input_process, **kwargs)
         self.sf_join_frequencies = set_default_unit(sf_join_frequencies, u.Hz)
         self.sf_components = sf_components
         self.sf_thr = sf_thr
         self.keep0 = keep0
@@ -228,14 +235,15 @@
         self.weight_across_epochs = weight_across_epochs
         self.plot_x_lim = plot_x_lim
         self.plot_y_lim = plot_y_lim
         self.user_naming_rule = user_naming_rule
         self.fig_format = fig_format
         self.return_figures = return_figures
         self.save_to_file = save_to_file
+        self.n_jobs = n_jobs
         self.__kwargs = kwargs
 
     def transform_data(self):
         figures = None
         if self.test_frequencies is None:
             self.test_frequencies = self.sf_join_frequencies
         if self.return_figures:
@@ -248,15 +256,16 @@
                                        weight_across_epochs=self.weight_across_epochs,
                                        keep0=self.keep0,
                                        keep1=self.keep1,
                                        perc0=self.perc0,
                                        perc1=self.perc1,
                                        block_size=self.block_size,
                                        n_tracked_points=self.n_tracked_points,
-                                       delta_frequency=self.delta_frequency
+                                       delta_frequency=self.delta_frequency,
+                                       n_jobs=self.n_jobs
                                        )
         spatial_filter.run()
         filtered_data = ApplySpatialFilter(input_process=spatial_filter,
                                            sf_components=self.sf_components,
                                            sf_thr=self.sf_thr,
                                            **self.__kwargs)
         filtered_data.run()
```

### Comparing `peegy-1.4.3/peegy/processing/pipe/statistics.py` & `peegy-1.4.4/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/storage.py` & `peegy-1.4.4/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/time_frequency.py` & `peegy-1.4.4/peegy/processing/pipe/time_frequency.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/pipe/bootstrap/bootstrap.py` & `peegy-1.4.4/peegy/processing/pipe/bootstrap/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,19 @@
                                                       miniters=0)]
             ray.shutdown()
             for _r in results:
                 bootstrapped_tables = bootstrapped_tables + _r
         elif backend == 'joblib':
             # multiprocessing bootstrap via joblib
             ref_data = self._origin_input_process.output_node.data.copy()
-            self._origin_input_process.input_node.data = None
-            self._origin_input_process.output_node.data = None
+            if self._origin_input_process.input_node is not None:
+                self._origin_input_process.input_node.data = None
+
+            if self._origin_input_process.output_node is not None:
+                self._origin_input_process.output_node.data = None
             for _, _value in self.at_each_bootstrap_do.items():
                 _value.input_node.data = None
                 _value.output_node.data = None
             reference_pool_id = self.at_each_bootstrap_do
             target_tables = self.bootstrap_targets
             # ref_process = copy.deepcopy(self._origin_input_process)
             ref_process = self._origin_input_process
```

### Comparing `peegy-1.4.3/peegy/processing/statistics/definitions.py` & `peegy-1.4.4/peegy/processing/statistics/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.4.4/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/system/progress.py` & `peegy-1.4.4/peegy/processing/system/progress.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.4.4/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Many of the functions here defined are originally published by Alain de Cheveigné
 http://audition.ens.fr/adc/NoiseTools/
 """
 import numpy as np
 import pyfftw
-import multiprocessing
 from tqdm import tqdm
 import astropy.units as u
 from peegy.tools.units.unit_tools import set_default_unit
+import numba
 __author__ = 'jaime undurraga'
 
 
 def et_covariance(x: np.array = np.array([]),
                   shifts: np.array(int) = np.array([0]),
                   w: np.array = np.array([])) -> (np.array, float):
     """
@@ -105,23 +105,25 @@
 
 
 def et_freq_shifted_xcovariance(x: np.array = np.array([]),
                                 y: np.array = np.array([]),
                                 shifts: np.array(int) = np.array([0]),
                                 wx: np.array = np.array([]),
                                 wy: np.array = np.array([]),
-                                normalized_frequencies: np.array = np.array([])) -> (np.array, float):
+                                normalized_frequencies: np.array = np.array([]),
+                                n_jobs: int = 1) -> (np.array, float):
     """
         Compute covariance matrix between x and y in the frequency domain
         :param x: numpy array with data
         :param y: numpy array with data
         :param shifts: integer array specifying shifts
         :param wx: numpy array with weights to be applied to x
         :param wy: numpy array with weights to be applied to y
         :param normalized_frequencies: normalized freqs to compute covariance
+        :param n_jobs: number of CPUs to compute FFT
         :return c: numpy array with covariance matrix
         :return tw: weights norm
         """
 
     n_shifts = shifts.size
     c = np.zeros((x.shape[1], y.shape[1] * n_shifts))
     if x.ndim == 2:
@@ -149,21 +151,25 @@
     tw = 0
     for i in np.arange(x.shape[2]):
         yy = et_multi_shift(y[:, :, i], shifts)
         wyy = et_multi_shift(wy[:, :, i], shifts)
         xx = x[0: yy.shape[0], :, i]
         wxx = wx[0: yy.shape[0], :, i]
         xx = xx * wxx
-        fftx = pyfftw.builders.rfft(xx, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                    threads=multiprocessing.cpu_count())
         yy = y[:, :, i] * wyy
-        ffty = pyfftw.builders.rfft(yy, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                    threads=multiprocessing.cpu_count())
-        xfft = fftx()
-        yfft = ffty()
+        xfft = pyfftw.builders.rfft(xx,
+                                    overwrite_input=False,
+                                    planner_effort='FFTW_ESTIMATE',
+                                    axis=0,
+                                    threads=n_jobs)()
+        yfft = pyfftw.builders.rfft(yy,
+                                    overwrite_input=False,
+                                    planner_effort='FFTW_ESTIMATE',
+                                    axis=0,
+                                    threads=n_jobs)()
         zx = xfft * freq_filt
         zy = yfft * freq_filt
         c = c + 2 * np.real(zx.T.conj().dot(zy))
         tw = tw + wxx.T.dot(wyy)
 
     return c, tw
 
@@ -232,14 +238,15 @@
 
 
 def et_x_join_covariance(x, y):
     # compute the covariance combining all epochs
     return et_unfold(x).T.dot(et_unfold(y))
 
 
+@numba.jit(nogil=True, nopython=True)
 def et_find_freq_bin(freq_vector: np.array = np.array([]),
                      freq_to_find: np.array = np.array([])):
     f_bins = []
     for f in freq_to_find:
         f_pos = np.argmin(np.abs(freq_vector - f))
         f_bins.append(f_pos)
     return f_bins
@@ -278,15 +285,16 @@
                 z[:, pos, k] = y[shift_array]
     z = z.squeeze()
     return z
 
 
 def et_freq_weighted_cov(x: np.array = np.array([]),
                          normalized_frequencies: np.array = np.array([]),
-                         w: np.array = np.array([])):
+                         w: np.array = np.array([]),
+                         n_jobs: int = 1):
     if x.ndim == 2:
         x = x[:, :, None]
     if np.mod(x.shape[0], 2) == 0:
         fft_size = int((x.shape[0] / 2) + 1)
     else:
         fft_size = int((x.shape[0] + 1) / 2)
 
@@ -297,21 +305,28 @@
     if w.size == 0:
         w = np.ones(x.shape)
         # w = w / np.sum(w, axis=2, keepdims=True)
     # normalize weights
     # w = w / np.sum(w ** 2, axis=2, keepdims=True)
     c = 0
     tw = 0
+    xfft = pyfftw.builders.rfft(x * w,
+                                overwrite_input=False,
+                                planner_effort='FFTW_ESTIMATE',
+                                axis=0,
+                                threads=n_jobs)()
+
     for i in tqdm(np.arange(x.shape[2]), desc='Spatial filter covariance estimation'):
         ww = w[:, :, i]
-        xx = x[:, :, i] * ww
-        fft = pyfftw.builders.rfft(xx, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                   threads=multiprocessing.cpu_count())
-        xfft = fft()
-        z = xfft * freq_filt
+        # xx = x[:, :, i] * ww
+        # fft = pyfftw.builders.rfft(xx, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
+        #                            threads=multiprocessing.cpu_count())
+        # xfft = fft()
+        # xfft = np.fft.rfft(xx, axis=0)
+        z = xfft[:, :, i] * freq_filt
         c = c + 2 * np.real(z.T.conj().dot(z))
         tw = tw + ww.T.dot(ww)
     return c, tw
 
 
 # def et_tsr(x: np.array = np.array([]),
 #            ref: np.array = np.array([]),
```

### Comparing `peegy-1.4.3/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.4.4/peegy/processing/tools/epochs_processing_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from peegy.processing.tools.multiprocessing.multiprocessesing_filter import filt_data
 from peegy.processing.tools.filters.eog_tools.tools import generate_eog_template, reconstruct_eog
 from sklearn import linear_model
 import matplotlib.pyplot as plt
 import peegy.processing.tools.filters.spatial_filtering.spatial_filtering as sf
 from peegy.processing.system.memory import enough_memory
 import pyfftw
-import multiprocessing
 from scipy import signal
 import pycwt as wavelet
 import pywt as pw
 from sklearn.linear_model import LinearRegression
 from peegy.tools.units.unit_tools import set_default_unit
 import astropy.units as u
 from tqdm import tqdm
@@ -143,25 +142,27 @@
 
 def et_mean(epochs: np.array = np.array([]),
             block_size: int = 10,
             samples_distance: int = 1,
             weighted: bool = True,
             normalize_weights: bool = False,
             demean_epochs: bool = True,
-            weight_across_epochs: bool = True):
+            weight_across_epochs: bool = True,
+            n_jobs: int = 1):
     """
     Compute the mean of the input epochs
     :param epochs: samples x channels x trials numpy array
     :param block_size: number of trials used to estimate noise and weights
     :param samples_distance: separation between samples to estimate noise and weights
     :param weighted: boolean indicating if weighted average is used
     :param normalize_weights: if true weights will be normalized so that their sum across x is equal to 1
     :param demean_epochs: if True, individual epochs will be demeaned
     :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights are
     computed within epoch (1 / variance across time)
+    :param n_jobs: number of CPUs to compute FFT
     :return: average data (standard or weighted), weights, residual noise, cumulative residual noise over trials,
     spectrum of final average scaled to time domain amplitudes, array with number of sources per noise source
     """
     epochs = set_default_unit(epochs, u.dimensionless_unscaled)
     if weighted:
         if weight_across_epochs:
             w, final_rn, cumulative_rn, n, wb, nb = et_get_epoch_weights_and_rn_weighted_average(
@@ -184,16 +185,19 @@
             demean_epochs=demean_epochs
         )
     # normalize weights to facilitate computations
     if normalize_weights:
         w = w / np.sum(w, axis=1)[:, None]
     w = np.tile(w, (epochs.shape[0], 1, 1))
     w_ave = eo.w_mean(epochs, w)
-    fft = pyfftw.builders.rfft(w_ave, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                               threads=multiprocessing.cpu_count())
+    fft = pyfftw.builders.rfft(w_ave,
+                               overwrite_input=False,
+                               planner_effort='FFTW_ESTIMATE',
+                               axis=0,
+                               threads=n_jobs)
     scaling_factor = 2 / epochs.shape[0]
     w_fft = fft() * scaling_factor * w_ave.unit
     snr = np.var(w_ave, ddof=1, axis=0) / final_rn ** 2 - 1
     return w_ave, w, final_rn, cumulative_rn, w_fft, n, wb, nb, snr
 
 
 def et_snr_in_rois(data: np.array = None,
@@ -368,41 +372,41 @@
 def et_frequency_mean2(epochs=np.array([]),
                        fs: u.Quantity = None,
                        block_size: int = 10,
                        test_frequencies: np.array = None,
                        scale_frequency_data: bool = True,
                        weighted_average: bool = True,
                        delta_frequency: u.Quantity = 2 * u.Hz,
-                       power_line_frequency: u.Quantity = 50 * u.Hz):
+                       power_line_frequency: u.Quantity = 50 * u.Hz,
+                       n_jobs: int = 1):
     epochs = set_default_unit(epochs, u.uV)
     fs = set_default_unit(fs, u.Hz)
     delta_frequency = set_default_unit(delta_frequency, u.Hz)
     test_frequencies = set_default_unit(test_frequencies, u.Hz)
 
     weights, pooled_rn, pooled_snr, by_freq_rn, by_freq_snr, freq_samples, exact_frequencies = \
         get_pooled_frequency_weights(
             epochs=epochs,
             fs=fs,
             block_size=block_size,
             frequencies=test_frequencies,
             weighted_average=weighted_average,
             delta_frequency=delta_frequency,
-            power_line_frequency=power_line_frequency,
+            power_line_frequency=power_line_frequency
         )
 
     w_ave = eo.w_mean(epochs=epochs,
                       weights=weights[0, :, :])
-
     fft = pyfftw.builders.rfft(w_ave, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                               threads=multiprocessing.cpu_count())
+                               threads=n_jobs)()
     scaling_factor = 1.0
     if scale_frequency_data:
         scaling_factor = 2 / epochs.shape[0]
 
-    w_fft = fft() * scaling_factor * w_ave.unit
+    w_fft = fft * scaling_factor * w_ave.unit
     freq_samples = scaling_factor * freq_samples
     pooled_rn = scaling_factor * pooled_rn
     return w_ave, pooled_snr, pooled_rn, by_freq_snr, by_freq_snr, w_fft, weights, freq_samples, exact_frequencies
 
 
 def et_subtract_correlated_ref(data: np.array = np.array([]),
                                idx_ref: np.array = np.array([]),
@@ -580,15 +584,16 @@
                              demean_data: bool = True,
                              keep0: int = None,
                              keep1: float = 1e-9,
                              perc0: float = 1,
                              perc1: float = None,
                              block_size: int = 10,
                              n_tracked_points: int = None,
-                             delta_frequency: u.Quantity = 5 * u.Hz
+                             delta_frequency: u.Quantity = 5 * u.Hz,
+                             n_jobs: int = 1,
                              ):
     """
 
     :param epochs: m x n x l (samples, channels, epochs)
     :param fs: sampling rate
     :param sf_join_frequencies: numpy array with frequencies to bias the filter
     :param weight_data: if True, covariance and mean will be estimated using weights
@@ -605,29 +610,30 @@
     :param perc0: float (between 0 and 1) controlling whitening of unbiased components in DSS.
     This value will preserve components that explain the percentage of variance.
     :param perc1: float (between 0 and 1) controlling the number of biased components kept in DSS.
     This value will preserve the components of the biased PCA analysis that explain the percentage of variance.
     :param block_size: integer indicating the number of trials that would be use to estimate the weights
     :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
     :param delta_frequency: frequency size around each sf_join_frequency to estimate noise
+    :param n_jobs: number of CPUs to compute FFT
     :return: z, pwr0, pwr1, cov_1, weights: components, unbiased power, biased power, covariance rotation,
     estimated weights
     """
     print('computing spatial filter')
 
     # bias function uses weighted mean or standard mean
     if weight_data and weights is None:
         if weighted_frequency_domain:
             weights, *_ = get_pooled_frequency_weights(
                 epochs=epochs,
                 fs=fs,
                 frequencies=sf_join_frequencies,
                 weighted_average=weight_data,
                 block_size=block_size,
-                delta_frequency=delta_frequency,
+                delta_frequency=delta_frequency
             )
         else:
             if n_tracked_points is None:
                 n_tracked_points = epochs.shape[0]
             samples_distance = int(max(epochs.shape[0] // n_tracked_points, 1))
             _, weights, *_ = et_mean(epochs,
                                      weighted=weight_data,
@@ -640,22 +646,29 @@
     if demean_data:
         epochs = eo.et_demean(epochs, w=weights)
 
     average = eo.w_mean(epochs, weights=weights)
 
     if sf_join_frequencies is not None:
         n_frequencies = sf_join_frequencies / fs
-        c0, t0 = eo.et_freq_weighted_cov(epochs, normalized_frequencies=n_frequencies, w=weights.value)
-        c1, t1 = eo.et_freq_weighted_cov(average, normalized_frequencies=n_frequencies)
+        c0, t0 = eo.et_freq_weighted_cov(epochs,
+                                         normalized_frequencies=n_frequencies,
+                                         w=weights.value,
+                                         n_jobs=n_jobs)
+        c1, t1 = eo.et_freq_weighted_cov(average,
+                                         normalized_frequencies=n_frequencies,
+                                         n_jobs=n_jobs)
         c0 = c0 / t0
         c1 = c1 / t1
         todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(c0, c1, keep0=keep0, keep1=keep1, perc0=perc0, perc1=perc1)
         z = eo.et_mmat(epochs, todss)
-        cov_1, tw_cov = eo.et_freq_shifted_xcovariance(z, epochs, normalized_frequencies=n_frequencies,
-                                                       wy=weights.value)
+        cov_1, tw_cov = eo.et_freq_shifted_xcovariance(z, epochs,
+                                                       normalized_frequencies=n_frequencies,
+                                                       wy=weights.value,
+                                                       n_jobs=n_jobs)
         cov_1 = cov_1 / tw_cov
     else:
         # clean data using dss with weighted average as bias. Data covariance weighted with same weights
         c0, tw0 = eo.et_weighted_covariance(epochs, w=weights.value)
         c1, tw1 = eo.et_weighted_covariance(average)
         c0 = c0 / tw0
         c1 = c1 / tw1
@@ -784,18 +797,19 @@
         print('Computing spectrogram {:} out of {:}'. format(_i, data.shape[2]))
     ave /= data.shape[2]
     return ave, time, freqs
 
 
 def et_average_frequency_transformation(epochs: np.array = np.array([]),
                                         fs=0.0,
-                                        ave_mode='magnitude'):
+                                        ave_mode='magnitude',
+                                        n_jobs: int = 1):
 
     fft = pyfftw.builders.rfft(epochs, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                               threads=multiprocessing.cpu_count())
+                               threads=n_jobs)
     _fft = fft()
 
     if ave_mode == 'magnitude':
         _fft = np.abs(_fft)
     ave = np.abs(np.mean(_fft, axis=2))
     ave *= 2/epochs.shape[0]
     freqs = np.arange(0, _fft.shape[0]) * fs / epochs.shape[0]
@@ -832,74 +846,76 @@
 def et_impulse_response_artifact_subtraction(
         data: np.array = None,
         stimulus_waveform: np.array = None,
         ir_length: int = 100,
         ir_max_lag: int = 0,
         regularization_factor: float = 1,
         plot_results: bool = False,
+        n_jobs: int = 1
 ) -> np.array:
     """
     This function will remove an artifact which has the shape of the input stimulus_waveform.
     Here, artifact is estimated from the impulse response. The latter is estimated by averaging individual
     impulse responses across epochs.
     :param data: data samples x channels x trials
     :param stimulus_waveform: single column numpy array with the target waveform artifact
     :param ir_length: estimated impulse response length in samples
     :param ir_max_lag: maximum lag or sydtem delay (from zero). Impulse response window will be centered around the max
     within the max_lag.
     :param regularization_factor: This value is used to regularize the deconvolution based on Tikhonov regularization
     allow to estimate the transfer function when the input signal is sparse in frequency components
     :param plot_results: if True, figures with results will be shown
+    :param n_jobs: number of CPUs to compute FFT
     :return: data without artifacts
     """
     original_data_shape = data.shape
     # compute impulse response; data padded to next power of 2 to speed process
     n_fft = next_power_two(data.shape[0])
 
     data = np.atleast_3d(data)
     _stim_template = stimulus_waveform[0: data.shape[0]]
     data = np.pad(data, ((0, n_fft - data.shape[0]), (0, 0), (0, 0)), constant_values=(0, 0), mode='constant')
     _stim_template = np.pad(_stim_template, ((0, n_fft - _stim_template.shape[0]), (0, 0)),
                             constant_values=(0, 0), mode='constant')
     _fft = pyfftw.builders.rfft(_stim_template,
                                 overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                threads=multiprocessing.cpu_count())
+                                threads=n_jobs)
     x_fft = _fft()
     _fft = pyfftw.builders.rfft(data,
                                 overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                threads=multiprocessing.cpu_count())
+                                threads=n_jobs)
     y_fft = _fft()
 
     # estimate impulse response for each epoch via Tikhonov regularization
     x_fft = np.atleast_3d(x_fft)
     h_fft = y_fft * np.conjugate(x_fft) / (x_fft * np.conjugate(x_fft) + regularization_factor)
 
     _ifft = pyfftw.builders.irfft(h_fft,
                                   n=data.shape[0],
                                   overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                  threads=multiprocessing.cpu_count())
+                                  threads=n_jobs)
     h = _ifft()
     h = np.mean(h, axis=2, keepdims=True)
     w = np.zeros(h.shape)
     ws = np.repeat(signal.windows.hanning(ir_length).reshape(-1, 1), h.shape[1], axis=1)
     w[0: ws.shape[0], :, :] = np.atleast_3d(ws)
     _max_ir = np.argmax(h[0: ir_max_lag + 1])
     w = np.roll(w, -ir_length // 2 + _max_ir, axis=0)
     h_ave_w = h * w
     # estimate artifact by convolution
     _fft = pyfftw.builders.rfft(h_ave_w,
                                 overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                threads=multiprocessing.cpu_count())
+                                threads=n_jobs)
     h_ave_w_fft = _fft()
     # convolve
     fft_artifact = h_ave_w_fft * x_fft
     _ifft = pyfftw.builders.irfft(fft_artifact,
                                   n=data.shape[0],
                                   overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                  threads=multiprocessing.cpu_count())
+                                  threads=n_jobs)
     _recovered_artifact = _ifft() * data.unit
     _clean_data = data - _recovered_artifact
     if plot_results:
         plt.figure()
         plt.plot(h.squeeze(), label='full IR')
         plt.plot(h_ave_w.squeeze(), label='windowed IR')
         plt.legend()
@@ -1253,37 +1269,42 @@
     exact_frequency = freqs[k]
     return real + 1j * imag, exact_frequency
 
 
 def discrete_dft(data: np.array = None,
                  fs: float = None,
                  frequencies: float = None,
-                 method: str = 'auto'):
+                 method: str = 'auto',
+                 n_jobs: int = 1):
     """
     Gets individual frequency Fourier values using either fast fft or Goertzel depending on available memory.
     :param data: (time x channels) numpy array
     :param fs: float indicating the sampling rate
     :param frequencies: frequencies to be estimated in Hz
     :param method: string specifying how to compute DFT
+    :param n_jobs: number of CPUs to comput FFT
     :return: np.array with Fourier frequency term for each channel (1 x channels)
     """
     data = set_default_unit(data, u.uV)
     frequencies = set_default_unit(frequencies, u.Hz)
     n = data.shape[0]
     freqs = np.arange(0, n) * fs / n
     k = np.array([np.argmin(np.abs(freqs - _f)) for _f in frequencies])
     dft = np.zeros((k.size, data.shape[1], data.shape[2])) * data.unit
     exact_frequencies = np.zeros(k.size) * frequencies.unit
     _memory = enough_memory(data)
     if method == 'auto':
         _method = 'fft' if _memory else 'goertzel'
 
     if _method == 'fft':
-        fft = pyfftw.builders.rfft(data, overwrite_input=False, planner_effort='FFTW_ESTIMATE', axis=0,
-                                   threads=multiprocessing.cpu_count())
+        fft = pyfftw.builders.rfft(data,
+                                   overwrite_input=False,
+                                   planner_effort='FFTW_ESTIMATE',
+                                   axis=0,
+                                   threads=n_jobs)
         _fft = fft()
         dft = _fft[k, :] * data.unit
         exact_frequencies = freqs[k]
     elif _method == 'goertzel':
         for _i, _f in enumerate(frequencies):
             _dft, _exact_frequency = goertzel(data, fs, _f)
             dft[_i] = _dft
```

### Comparing `peegy-1.4.3/peegy/processing/tools/weightedAverage.py` & `peegy-1.4.4/peegy/processing/tools/weightedAverage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/detection/definitions.py` & `peegy-1.4.4/peegy/processing/tools/detection/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.4.4/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.4.4/peegy/processing/tools/filters/eegFiltering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/filters/resampling.py` & `peegy-1.4.4/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.4.4/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py` & `peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.4.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.4.4/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/template_generator/h0.json` & `peegy-1.4.4/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/processing/tools/video/recording.py` & `peegy-1.4.4/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/dss_unit_tests.py` & `peegy-1.4.4/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/eeg_test_resampling.py` & `peegy-1.4.4/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/javerager_test.py` & `peegy-1.4.4/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/read_data_test.py` & `peegy-1.4.4/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_assr_moving_average.py` & `peegy-1.4.4/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_average_spectrogram_power.py` & `peegy-1.4.4/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_biosemi_class.py` & `peegy-1.4.4/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_biosemi_reader.py` & `peegy-1.4.4/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_bootstraping.py` & `peegy-1.4.4/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_edf_reader.py` & `peegy-1.4.4/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_eeg_notch_filter.py` & `peegy-1.4.4/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_eog_removal_correlation.py` & `peegy-1.4.4/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_eog_template_removal.py` & `peegy-1.4.4/peegy/test/test_eog_template_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.4.4/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_et_tools.py` & `peegy-1.4.4/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_filter.py` & `peegy-1.4.4/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_fir_filter_mt.py` & `peegy-1.4.4/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_fir_filter_ols.py` & `peegy-1.4.4/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_fiter_mt.py` & `peegy-1.4.4/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_freq_noise_estimation.py` & `peegy-1.4.4/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_freq_noise_estimation_plots.py` & `peegy-1.4.4/peegy/test/test_freq_noise_estimation_plots.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_frequency_average_epochs.py` & `peegy-1.4.4/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_hotelling_t2.py` & `peegy-1.4.4/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_ica_average_epochs.py` & `peegy-1.4.4/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_multiprocessing.py` & `peegy-1.4.4/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_noise_generator.py` & `peegy-1.4.4/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_norm_corr.py` & `peegy-1.4.4/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_peakdetection.py` & `peegy-1.4.4/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_phase_locking_value.py` & `peegy-1.4.4/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.4.4/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_scrolling.py` & `peegy-1.4.4/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.4.4/peegy/test/test_spatial_filtering_example1.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.4.4/peegy/test/test_spatial_filtering_example6.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_w_average_epochs.py` & `peegy-1.4.4/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/artifact_removal/ir_test.py` & `peegy-1.4.4/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.4.4/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.4.4/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat` & `peegy-1.4.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.4.4/peegy/tools/signal_generator/noise_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import numpy as np
 import math
+from scipy.signal import firwin2
+# from scipy.signal import freqz
+from peegy.processing.tools.multiprocessing .multiprocessesing_filter import filt_data
+import astropy.units as u
 
 
 def rms(signal):
     return np.mean(signal ** 2.0, axis=0) ** 0.5
 
 
 def lcm(num1, num2):
@@ -55,15 +59,18 @@
                              f_noise_low: float = 300.0,
                              f_noise_high: float = 700.0,
                              attenuation: float = 0.0,
                              modulation_frequency: float = 0.0,
                              modulation_phase: float = 0.0,
                              modulation_index: float = 0.0,
                              reference_rms: bool = None,
-                             noise_seed=None):
+                             noise_seed=None,
+                             frequency_domain=False,
+                             freq_resolution: float = 0.1,
+                             n_taps: int = None):
     """
     This function generates coloured noise (1 / f ** p) in the frequency-domain.
     :param fs:  sampling rate
     :param duration: duration in seconds
     :param n_channels: number of output channels
     :param n_repetitions: how many times to repeat the time series (output is equal to duration * n_repetitions)
     :param amplitude: output maximum amplitude (between -1 and 1)
@@ -71,14 +78,19 @@
     :param f_noise_high: high frequency cutoff frequency
     :param attenuation: decay of power spectral density in dB / octave (3 dB for pink noise, 6 dB for brown noise)
     :param modulation_frequency: frequency in Hz to apply a temporal modulation to the noise
     :param modulation_phase: starting phase (in radians) of the modulation frequency
     :param modulation_index: value between 0 (un-modulated) and 1 (full modulated)
     :param reference_rms: rms value to apply in case of this value has been calculated to produced calibrated sounds
     :param noise_seed: float to initialize the random generator
+    :param frequency_domain: if True, the noise is generated by randomizing the phase of the frequency components. If
+    false, a FIR filter is estimated and applied to a random noise
+    :param n_taps: integer indicating number of filter tabs in case of frequency_domain=False
+    :param freq_resolution: frequency resolution to create FIR filter. If n_tabs is not passed, then number of tabs is
+    computed to ensure the frequency resolution passed.
     :return: noise waveform (samples x channels)
     """
     if noise_seed is not None:
         np.random.seed(noise_seed)
     time = np.expand_dims(np.arange(0, np.round(fs * duration)) / fs, axis=1)
     n = time.size
     if np.mod(n, 2) == 0:
@@ -89,21 +101,43 @@
     freq = np.arange(0, n_uniq_freq).reshape([-1, 1]) * fs / n
     p = -attenuation / (10 * np.log10(0.5))
     psd_noise = np.zeros((n_uniq_freq, 1))
 
     # synthesize power spectral density
     _idx_power = np.argwhere(np.logical_and(freq >= f_noise_low, freq <= f_noise_high))[:, 0]
     psd_noise[_idx_power] = 1 / (1 + freq[_idx_power] ** p)
-
+    # ensure odd number of taps
+    if n_taps is not None:
+        n_taps = 2 * (n_taps // 2) + 1
     # synthesize phase
-    phase_noise = 2 * np.pi * np.random.rand(n_uniq_freq, n_channels)
-    spectrum_noise = np.sqrt(psd_noise) * np.exp(1j * phase_noise)
-
-    # synthesize noise in the time-domain
-    noise = np.fft.irfft(spectrum_noise, n, axis=0)
+    if not frequency_domain:
+        gain = np.sqrt(psd_noise)
+        if freq_resolution is not None:
+            n_taps = int(np.maximum(1, n // np.floor(freq_resolution / (fs / n))))
+            n_taps = 2 * (n_taps // 2) + 1
+        # force last frequency to be fs / 2
+        freq[-1, :] = fs / 2
+        print('noise generation: {:} taps FIR design'.format(n_taps))
+        _b = firwin2(numtaps=n_taps,
+                     freq=freq[:, 0],
+                     fs=fs,
+                     gain=gain[:, 0],
+                     antisymmetric=False)
+        white_noise = np.random.rand(n, n_channels)
+        noise = filt_data(b=_b, data=white_noise * u.dimensionless_unscaled, mode='original').value
+        # plot results
+        # f, h = freqz(_b, worN=np.linspace(0, fs / 2, n_taps), fs=fs)
+        # import matplotlib.pyplot as plt
+        # plt.plot(f, 20 * np.log10(np.abs(h)), label='Filter response')
+        # plt.plot(freq.flatten(), 20 * np.log10(gain), label='Target response')
+    else:
+        phase_noise = 2 * np.pi * np.random.rand(n_uniq_freq, n_channels)
+        spectrum_noise = np.sqrt(psd_noise) * np.exp(1j * phase_noise)
+        # synthesize noise in the time-domain
+        noise = np.fft.irfft(spectrum_noise, n, axis=0)
 
     # modulated noise
     mod_amp = (1 - modulation_index * np.cos(2 * np.pi * modulation_frequency * time + modulation_phase)) / \
               (1 + modulation_index)
     _amplitude = amplitude * mod_amp
     noise = noise / np.max(np.abs(noise), axis=0)
     noise = _amplitude * noise
```

### Comparing `peegy-1.4.3/peegy/tools/units/unit_tools.py` & `peegy-1.4.4/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/LICENSE.txt` & `peegy-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.4.3/pyproject.toml` & `peegy-1.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel", "hatchling"]
 build-backend = "hatchling.build"
 #build-backend = "setuptools.build_meta"
 
 [project]
 name = "peegy"
-version = "1.4.3"
+version = "1.4.4"
 authors = [{name = "Jaime Undurraga", email = "jaime.undurraga@gmail.com"},]
 description = "Tools to pipeline bulk analyses of EEG and other modalities."
 requires-python = ">=3.9"
 license = {text = "MIT"}
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `peegy-1.4.3/PKG-INFO` & `peegy-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Project-URL: Homepage, https://gitlab.com/open-source-brain/peegy/
 Project-URL: Examples, https://open-source-brain.gitlab.io/peegy/
 Author-email: Jaime Undurraga <jaime.undurraga@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
```

