# Comparing `tmp/mne-1.4.1.tar.gz` & `tmp/mne-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-1.4.1.tar", last modified: Mon Jun  5 16:28:42 2023, max compression
+gzip compressed data, was "mne-1.4.2.tar", last modified: Tue Jun  6 14:44:59 2023, max compression
```

## Comparing `mne-1.4.1.tar` & `mne-1.4.2.tar`

### file list

```diff
@@ -1,1243 +1,1243 @@
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.252119 mne-1.4.1/
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.029056 mne-1.4.1/.circleci/
--rw-r--r--   0 larsoner   (501) staff       (20)    18220 2023-06-05 16:25:38.000000 mne-1.4.1/.circleci/config.yml
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.029889 mne-1.4.1/.github/
--rw-r--r--   0 larsoner   (501) staff       (20)      935 2022-11-28 17:38:20.000000 mne-1.4.1/.github/CODEOWNERS
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.030628 mne-1.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 larsoner   (501) staff       (20)     1933 2022-11-28 17:38:20.000000 mne-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 larsoner   (501) staff       (20)      258 2022-11-28 17:38:20.000000 mne-1.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 larsoner   (501) staff       (20)      900 2022-11-28 17:38:20.000000 mne-1.4.1/.github/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0 larsoner   (501) staff       (20)     1633 2022-11-28 17:38:20.000000 mne-1.4.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 larsoner   (501) staff       (20)     1004 2023-06-05 14:01:41.000000 mne-1.4.1/.github/config.yml
--rw-r--r--   0 larsoner   (501) staff       (20)      118 2022-11-28 17:38:20.000000 mne-1.4.1/.github/dependabot.yml
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.031121 mne-1.4.1/.github/workflows/
--rw-r--r--   0 larsoner   (501) staff       (20)      575 2023-06-05 14:01:41.000000 mne-1.4.1/.github/workflows/circle_artifacts.yml
--rw-r--r--   0 larsoner   (501) staff       (20)     2742 2022-11-28 17:38:20.000000 mne-1.4.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 larsoner   (501) staff       (20)     3593 2023-06-05 14:01:41.000000 mne-1.4.1/.github/workflows/tests.yml
--rw-r--r--   0 larsoner   (501) staff       (20)     1057 2023-06-05 14:01:41.000000 mne-1.4.1/.gitignore
--rw-r--r--   0 larsoner   (501) staff       (20)     1527 2022-11-28 17:38:20.000000 mne-1.4.1/LICENSE.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2534 2023-06-05 14:01:41.000000 mne-1.4.1/MANIFEST.in
--rw-r--r--   0 larsoner   (501) staff       (20)     6944 2023-06-05 16:28:42.251968 mne-1.4.1/PKG-INFO
--rw-r--r--   0 larsoner   (501) staff       (20)     5607 2023-06-05 14:01:41.000000 mne-1.4.1/README.rst
--rw-r--r--   0 larsoner   (501) staff       (20)     1343 2023-06-05 14:01:41.000000 mne-1.4.1/SECURITY.md
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.031338 mne-1.4.1/examples/
--rw-r--r--   0 larsoner   (501) staff       (20)      794 2022-11-28 17:38:20.000000 mne-1.4.1/examples/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.031560 mne-1.4.1/examples/connectivity/
--rw-r--r--   0 larsoner   (501) staff       (20)      326 2022-11-28 17:38:20.000000 mne-1.4.1/examples/connectivity/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.032800 mne-1.4.1/examples/datasets/
--rw-r--r--   0 larsoner   (501) staff       (20)      102 2022-05-20 17:14:56.000000 mne-1.4.1/examples/datasets/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2095 2023-06-05 14:01:41.000000 mne-1.4.1/examples/datasets/brainstorm_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)      737 2023-06-05 14:01:41.000000 mne-1.4.1/examples/datasets/hf_sef_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10907 2023-06-05 14:01:41.000000 mne-1.4.1/examples/datasets/limo_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4484 2023-06-05 14:01:41.000000 mne-1.4.1/examples/datasets/opm_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4287 2023-06-05 14:01:41.000000 mne-1.4.1/examples/datasets/spm_faces_dataset_sgskip.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.034821 mne-1.4.1/examples/decoding/
--rw-r--r--   0 larsoner   (501) staff       (20)      157 2022-05-20 17:14:56.000000 mne-1.4.1/examples/decoding/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     4745 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_csp_eeg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5964 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_csp_timefreq.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6879 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_rsa_sgskip.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4241 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_spatio_temporal_source.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2969 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_spoc_CMC.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3496 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_time_generalization_conditions.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2462 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_unsupervised_spatial_filter.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3912 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/decoding_xdawn_eeg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4727 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/ems_filtering.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4035 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/linear_model_patterns.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10675 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/receptive_field_mtrf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4816 2023-06-05 14:01:41.000000 mne-1.4.1/examples/decoding/ssd_spatial_filters.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.035518 mne-1.4.1/examples/forward/
--rw-r--r--   0 larsoner   (501) staff       (20)      143 2022-05-20 17:14:56.000000 mne-1.4.1/examples/forward/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     3718 2023-06-05 14:01:41.000000 mne-1.4.1/examples/forward/forward_sensitivity_maps.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2135 2023-06-05 14:01:41.000000 mne-1.4.1/examples/forward/left_cerebellum_volume_source.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2611 2023-06-05 14:01:41.000000 mne-1.4.1/examples/forward/source_space_morphing.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.040925 mne-1.4.1/examples/inverse/
--rw-r--r--   0 larsoner   (501) staff       (20)      168 2022-05-20 17:14:56.000000 mne-1.4.1/examples/inverse/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     4119 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/compute_mne_inverse_epochs_in_label.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1641 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/compute_mne_inverse_raw_in_label.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1680 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/compute_mne_inverse_volume.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6385 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/custom_inverse_solver.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4304 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/dics_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3461 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/dics_source_power.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5649 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/evoked_ers_source_power.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3193 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/gamma_map_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2073 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/label_activation_from_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3785 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/label_from_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3449 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/label_source_activations.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4774 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/mixed_norm_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5692 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/mixed_source_space_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4872 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/mne_cov_power.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5790 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/morph_surface_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6119 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/morph_volume_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7462 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/multi_dipole_model.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3411 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/multidict_reweighted_tfmxne.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7183 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/psf_ctf_label_leakage.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3190 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/psf_ctf_vertices.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4888 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/psf_ctf_vertices_lcmv.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3005 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/psf_volume.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1678 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/rap_music.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1467 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/read_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)      760 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/read_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4791 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/resolution_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5248 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/resolution_metrics_eegmeg.py
--rw-r--r--   0 larsoner   (501) staff       (20)      780 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/snr_estimate.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2489 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/source_space_snr.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5042 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/time_frequency_mixed_norm_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1704 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/trap_music.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3671 2023-06-05 14:01:41.000000 mne-1.4.1/examples/inverse/vector_mne_solution.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.041863 mne-1.4.1/examples/io/
--rw-r--r--   0 larsoner   (501) staff       (20)      262 2022-11-28 17:38:20.000000 mne-1.4.1/examples/io/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2073 2023-06-05 14:01:41.000000 mne-1.4.1/examples/io/elekta_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1356 2023-06-05 14:01:41.000000 mne-1.4.1/examples/io/read_neo_format.py
--rw-r--r--   0 larsoner   (501) staff       (20)      654 2023-06-05 14:01:41.000000 mne-1.4.1/examples/io/read_noise_covariance_matrix.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1193 2023-06-05 14:01:41.000000 mne-1.4.1/examples/io/read_xdf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.045342 mne-1.4.1/examples/preprocessing/
--rw-r--r--   0 larsoner   (501) staff       (20)      697 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2309 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/contralateral_referencing.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3808 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/css.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3162 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/define_target_events.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17460 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/eeg_bridging.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2934 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/eeg_csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1405 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/eog_artifact_histogram.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2407 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/eog_regression.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4818 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/find_ref_artifacts.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3096 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/fnirs_artifact_removal.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1497 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/ica_comparison.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1453 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/interpolate_bad_channels.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2908 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/movement_compensation.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3516 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/movement_detection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3021 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/muscle_detection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4382 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/muscle_ica.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2936 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/otp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1304 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/shift_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1608 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/virtual_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2593 2023-06-05 14:01:41.000000 mne-1.4.1/examples/preprocessing/xdawn_denoising.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.046220 mne-1.4.1/examples/simulation/
--rw-r--r--   0 larsoner   (501) staff       (20)       69 2022-05-20 17:14:56.000000 mne-1.4.1/examples/simulation/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     8699 2023-06-05 14:01:41.000000 mne-1.4.1/examples/simulation/plot_stc_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2450 2023-06-05 14:01:41.000000 mne-1.4.1/examples/simulation/simulate_evoked_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2820 2023-06-05 14:01:41.000000 mne-1.4.1/examples/simulation/simulate_raw_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8569 2023-06-05 14:01:41.000000 mne-1.4.1/examples/simulation/simulated_raw_data_using_subject_anatomy.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3293 2023-06-05 14:01:41.000000 mne-1.4.1/examples/simulation/source_simulator.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.047084 mne-1.4.1/examples/stats/
--rw-r--r--   0 larsoner   (501) staff       (20)      110 2022-05-20 17:14:56.000000 mne-1.4.1/examples/stats/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2640 2023-06-05 14:01:41.000000 mne-1.4.1/examples/stats/cluster_stats_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2501 2023-06-05 14:01:41.000000 mne-1.4.1/examples/stats/fdr_stats_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2404 2023-06-05 14:01:41.000000 mne-1.4.1/examples/stats/linear_regression_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2268 2023-06-05 14:01:41.000000 mne-1.4.1/examples/stats/sensor_permutation_test.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3759 2023-06-05 14:01:41.000000 mne-1.4.1/examples/stats/sensor_regression.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.049085 mne-1.4.1/examples/time_frequency/
--rw-r--r--   0 larsoner   (501) staff       (20)      129 2022-05-20 17:14:56.000000 mne-1.4.1/examples/time_frequency/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     3857 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/compute_csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3165 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/compute_source_psd_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3682 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/source_label_time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1814 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/source_power_spectrum.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7980 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/source_power_spectrum_opm.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2179 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/source_space_time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1791 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/temporal_whitening.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7949 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/time_frequency_erds.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4999 2023-06-05 14:01:41.000000 mne-1.4.1/examples/time_frequency/time_frequency_global_field_power.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9775 2023-06-05 16:25:38.000000 mne-1.4.1/examples/time_frequency/time_frequency_simulated.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.052308 mne-1.4.1/examples/visualization/
--rw-r--r--   0 larsoner   (501) staff       (20)     4787 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/3d_to_2d.py
--rw-r--r--   0 larsoner   (501) staff       (20)       69 2022-05-20 17:14:56.000000 mne-1.4.1/examples/visualization/README.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     4312 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/brain.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2476 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/channel_epochs_image.py
--rw-r--r--   0 larsoner   (501) staff       (20)      908 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/eeg_on_scalp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2673 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/evoked_arrowmap.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6656 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/evoked_topomap.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2677 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/evoked_whitening.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1970 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/meg_sensors.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1319 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/mne_helmet.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2100 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/montage_sgskip.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2044 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/parcellation.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10240 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/publication_figure.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3156 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/roi_erpimage_by_rt.py
--rw-r--r--   0 larsoner   (501) staff       (20)      772 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/sensor_noise_level.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1224 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/ssp_projs_sensitivity_map.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1692 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/topo_compare_conditions.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1909 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/topo_customized.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1391 2023-06-05 14:01:41.000000 mne-1.4.1/examples/visualization/xhemi.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.063841 mne-1.4.1/mne/
--rw-r--r--   0 larsoner   (501) staff       (20)     5666 2023-06-05 16:25:38.000000 mne-1.4.1/mne/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      144 2023-06-05 14:01:41.000000 mne-1.4.1/mne/__main__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    27654 2023-06-05 14:01:41.000000 mne-1.4.1/mne/_freesurfer.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19447 2023-06-05 14:01:41.000000 mne-1.4.1/mne/_ola.py
--rw-r--r--   0 larsoner   (501) staff       (20)      176 2023-06-05 16:28:41.000000 mne-1.4.1/mne/_version.py
--rw-r--r--   0 larsoner   (501) staff       (20)    63163 2023-06-05 14:01:41.000000 mne-1.4.1/mne/annotations.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6831 2023-06-05 16:25:38.000000 mne-1.4.1/mne/baseline.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.066745 mne-1.4.1/mne/beamformer/
--rw-r--r--   0 larsoner   (501) staff       (20)      474 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20475 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/_compute_beamformer.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21949 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/_dics.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15860 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/_lcmv.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10057 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/_rap_music.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2833 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/resolution_matrix.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.067801 mne-1.4.1/mne/beamformer/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/beamformer/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    35200 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/tests/test_dics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4171 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/tests/test_external.py
--rw-r--r--   0 larsoner   (501) staff       (20)    42658 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/tests/test_lcmv.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8040 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/tests/test_rap_music.py
--rwxr-xr-x   0 larsoner   (501) staff       (20)     3313 2023-06-05 14:01:41.000000 mne-1.4.1/mne/beamformer/tests/test_resolution_matrix.py
--rw-r--r--   0 larsoner   (501) staff       (20)    86946 2023-06-05 14:01:41.000000 mne-1.4.1/mne/bem.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.070747 mne-1.4.1/mne/channels/
--rw-r--r--   0 larsoner   (501) staff       (20)     1854 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3120 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/_dig_montage_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14208 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/_standard_montage_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    84931 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/channels.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.014639 mne-1.4.1/mne/channels/data/
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.074875 mne-1.4.1/mne/channels/data/layouts/
--rw-r--r--   0 larsoner   (501) staff       (20)    14061 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/CTF-275.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     7154 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/CTF151.lay
--rw-r--r--   0 larsoner   (501) staff       (20)    12807 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/CTF275.lay
--rw-r--r--   0 larsoner   (501) staff       (20)    15343 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/EEG1005.lay
--rw-r--r--   0 larsoner   (501) staff       (20)    15526 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/EGI256.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     5823 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/GeodesicHeadWeb-130.lout
--rw-r--r--   0 larsoner   (501) staff       (20)    12573 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/GeodesicHeadWeb-280.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     6036 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/layouts/KIT-125.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     7562 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/KIT-157.lout
--rw-r--r--   0 larsoner   (501) staff       (20)    10895 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/layouts/KIT-160.lay
--rw-r--r--   0 larsoner   (501) staff       (20)    10020 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/KIT-AD.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     7572 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/KIT-AS-2008.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     7572 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/KIT-UMD-3.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     4406 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/layouts/Neuromag_122.lout
--rw-r--r--   0 larsoner   (501) staff       (20)    16054 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/Vectorview-all.lout
--rw-r--r--   0 larsoner   (501) staff       (20)    10704 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/Vectorview-grad.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     5256 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/Vectorview-grad_norm.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     5358 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/Vectorview-mag.lout
--rw-r--r--   0 larsoner   (501) staff       (20)     2770 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/layouts/biosemi.lay
--rw-r--r--   0 larsoner   (501) staff       (20)    11940 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/layouts/magnesWH3600.lout
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.079683 mne-1.4.1/mne/channels/data/montages/
--rw-r--r--   0 larsoner   (501) staff       (20)    24999 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/EGI_256.csd
--rw-r--r--   0 larsoner   (501) staff       (20)     5297 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-128.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     5316 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-129.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     7796 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-256.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     7823 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-257.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     1382 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-32.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     2877 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-64_1.0.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)     2919 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-65_1.0.sfp
--rw-r--r--   0 larsoner   (501) staff       (20)      544 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/montages/artinis-brite23.elc
--rw-r--r--   0 larsoner   (501) staff       (20)      376 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/montages/artinis-octamon.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     1555 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi128.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      248 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi16.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     1910 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi160.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     3354 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi256.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      453 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi32.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      710 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/biosemi64.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2358 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/montages/brainproducts-RNP-BA-128.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      947 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/easycap-M1.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      800 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/easycap-M10.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2110 2023-04-21 22:27:15.000000 mne-1.4.1/mne/channels/data/montages/mgh60.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     2428 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/montages/mgh70.elc
--rw-r--r--   0 larsoner   (501) staff       (20)    10478 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_1005.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     2896 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_1020.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     2009 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_alphabetic.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     3066 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_postfixed.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     2305 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_prefixed.elc
--rw-r--r--   0 larsoner   (501) staff       (20)     3093 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/montages/standard_primed.elc
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.085741 mne-1.4.1/mne/channels/data/neighbors/
--rw-r--r--   0 larsoner   (501) staff       (20)     4939 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-157_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     6636 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-208_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4990 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-NYU-2019_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4750 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-1_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4832 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-2_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4794 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-3_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4840 2022-11-28 17:38:12.000000 mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-4_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)      487 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/data/neighbors/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      511 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/biosemi16_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)      942 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/biosemi32_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1812 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/biosemi64_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     3920 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/bti148_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     6577 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/bti248_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     8337 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/bti248grad_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4380 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/ctf151_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     7831 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/ctf275_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2397 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/ctf64_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     3870 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycap128ch-avg_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1127 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycap32ch-avg_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1861 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycap64ch-avg_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1792 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycapM11_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     3529 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycapM14_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     3906 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycapM15_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2149 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/easycapM1_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     6286 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/ecog256_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4221 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/ecog256bipolar_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2422 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/eeg1010_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)    11892 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/elec1005_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2390 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/elec1010_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)      655 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/elec1020_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4045 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/itab153_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)      743 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/itab28_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1135 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/language29ch-avg_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     1660 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/mpi_59_channels_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2074 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/neuromag122cmb_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     3685 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/neuromag306cmb_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     2753 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/neuromag306mag_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     5580 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/neuromag306planar_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     4729 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/yokogawa160_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)    15521 2022-11-28 17:38:21.000000 mne-1.4.1/mne/channels/data/neighbors/yokogawa440_neighb.mat
--rw-r--r--   0 larsoner   (501) staff       (20)     8789 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/interpolation.py
--rw-r--r--   0 larsoner   (501) staff       (20)    39984 2023-06-05 16:25:38.000000 mne-1.4.1/mne/channels/layout.py
--rw-r--r--   0 larsoner   (501) staff       (20)    59199 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/montage.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.087220 mne-1.4.1/mne/channels/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/channels/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26410 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/tests/test_channels.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12511 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/tests/test_interpolation.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15138 2023-06-05 16:25:38.000000 mne-1.4.1/mne/channels/tests/test_layout.py
--rw-r--r--   0 larsoner   (501) staff       (20)    72846 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/tests/test_montage.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10249 2023-06-05 14:01:41.000000 mne-1.4.1/mne/channels/tests/test_standard_montage.py
--rw-r--r--   0 larsoner   (501) staff       (20)    55540 2023-06-05 14:01:41.000000 mne-1.4.1/mne/chpi.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.091132 mne-1.4.1/mne/commands/
--rw-r--r--   0 larsoner   (501) staff       (20)       51 2022-05-20 17:14:56.000000 mne-1.4.1/mne/commands/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3283 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_anonymize.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5425 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_browse_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3297 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_bti2fiff.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5876 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_clean_eog_ecg.py
--rw-r--r--   0 larsoner   (501) staff       (20)      538 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_compare_fiff.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8344 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_compute_proj_ecg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8354 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_compute_proj_eog.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3904 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5131 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_flash_bem.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3294 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_freeview_bem_surfaces.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2700 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_kit2fiff.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2503 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_make_scalp_surfaces.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6362 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_maxfilter.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1654 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_prepare_bem_model.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6116 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_report.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4224 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_setup_forward_model.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4982 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_setup_source_space.py
--rw-r--r--   0 larsoner   (501) staff       (20)      783 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_show_fiff.py
--rw-r--r--   0 larsoner   (501) staff       (20)      695 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_show_info.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1212 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_surf2bem.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1177 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_sys_info.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3196 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_watershed_bem.py
--rw-r--r--   0 larsoner   (501) staff       (20)      473 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/mne_what.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.091410 mne-1.4.1/mne/commands/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/commands/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16859 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/tests/test_commands.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3102 2023-06-05 14:01:41.000000 mne-1.4.1/mne/commands/utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    35658 2023-06-05 16:25:38.000000 mne-1.4.1/mne/conftest.py
--rw-r--r--   0 larsoner   (501) staff       (20)    78521 2023-06-05 14:01:41.000000 mne-1.4.1/mne/coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    80732 2023-06-05 14:01:41.000000 mne-1.4.1/mne/cov.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12277 2023-06-05 14:01:41.000000 mne-1.4.1/mne/cuda.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.097598 mne-1.4.1/mne/data/
--rw-r--r--   0 larsoner   (501) staff       (20)    84835 2022-11-28 17:38:21.000000 mne-1.4.1/mne/data/FreeSurferColorLUT.txt
--rw-r--r--   0 larsoner   (501) staff       (20)       23 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    51080 2022-11-28 17:38:21.000000 mne-1.4.1/mne/data/coil_def.dat
--rw-r--r--   0 larsoner   (501) staff       (20)     5064 2022-11-28 17:38:12.000000 mne-1.4.1/mne/data/coil_def_Elekta.dat
--rw-r--r--   0 larsoner   (501) staff       (20)   293567 2022-11-28 17:38:21.000000 mne-1.4.1/mne/data/eegbci_checksums.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     3419 2022-11-28 17:38:12.000000 mne-1.4.1/mne/data/extinction_coef.mat
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.100607 mne-1.4.1/mne/data/fsaverage/
--rw-r--r--   0 larsoner   (501) staff       (20)      260 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/fsaverage/fsaverage-fiducials.fif
--rw-r--r--   0 larsoner   (501) staff       (20)    97892 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/fsaverage/fsaverage-head.fif
--rw-r--r--   0 larsoner   (501) staff       (20)   491944 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/fsaverage/fsaverage-inner_skull-bem.fif
--rw-r--r--   0 larsoner   (501) staff       (20)      212 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/fsaverage/fsaverage-trans.fif
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.102105 mne-1.4.1/mne/data/helmets/
--rw-r--r--   0 larsoner   (501) staff       (20)     4706 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/122m.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)     9462 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/306m.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)     9443 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/306m_rt.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)    59505 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/BabySQUID.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)    11157 2022-11-28 17:38:12.000000 mne-1.4.1/mne/data/helmets/CTF_275.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)     9477 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/KIT.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)     9470 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/Magnes_2500wh.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)     9475 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/helmets/Magnes_3600wh.fif.gz
--rw-r--r--   0 larsoner   (501) staff       (20)  3732551 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/icos.fif.gz
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.102411 mne-1.4.1/mne/data/image/
--rw-r--r--   0 larsoner   (501) staff       (20)    11190 2022-11-28 17:38:21.000000 mne-1.4.1/mne/data/image/custom_layout.lout
--rw-r--r--   0 larsoner   (501) staff       (20)    12051 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/image/mni_brain.gif
--rw-r--r--   0 larsoner   (501) staff       (20)     4320 2022-05-20 17:14:56.000000 mne-1.4.1/mne/data/mne_analyze.sel
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.103353 mne-1.4.1/mne/datasets/
--rw-r--r--   0 larsoner   (501) staff       (20)     1620 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/__init__.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.104380 mne-1.4.1/mne/datasets/_fake/
--rw-r--r--   0 larsoner   (501) staff       (20)       75 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/_fake/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      844 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/_fake/_fake.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11863 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/_fetch.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.105023 mne-1.4.1/mne/datasets/_fsaverage/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/_fsaverage/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4563 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/_fsaverage/base.py
--rw-r--r--   0 larsoner   (501) staff       (20)      320 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/_fsaverage/bem.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     5795 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/_fsaverage/root.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.107656 mne-1.4.1/mne/datasets/_infant/
--rw-r--r--   0 larsoner   (501) staff       (20)     2499 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS1-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2475 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS10-5Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS12-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS15-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS18-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2499 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS2-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2493 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS2-0Weeks3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2677 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS2-0Years3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS3-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS4-5Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS6-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS7-5Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_infant/ANTS9-0Months3T.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     3866 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/_infant/base.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.108100 mne-1.4.1/mne/datasets/_phantom/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_phantom/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1834 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/_phantom/base.py
--rw-r--r--   0 larsoner   (501) staff       (20)      113 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/_phantom/phantom_otaniemi.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.109082 mne-1.4.1/mne/datasets/brainstorm/
--rw-r--r--   0 larsoner   (501) staff       (20)      114 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1789 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/bst_auditory.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1263 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/bst_phantom_ctf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1281 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/bst_phantom_elekta.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2298 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/bst_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1335 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/brainstorm/bst_resting.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13748 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/config.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.109367 mne-1.4.1/mne/datasets/eegbci/
--rw-r--r--   0 larsoner   (501) staff       (20)       97 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/eegbci/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7973 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/eegbci/eegbci.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.109519 mne-1.4.1/mne/datasets/eegbci/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)      397 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/eegbci/tests/test_eegbci.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.109900 mne-1.4.1/mne/datasets/epilepsy_ecog/
--rw-r--r--   0 larsoner   (501) staff       (20)       77 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/epilepsy_ecog/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      820 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/epilepsy_ecog/_data.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.110300 mne-1.4.1/mne/datasets/erp_core/
--rw-r--r--   0 larsoner   (501) staff       (20)       74 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/erp_core/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      682 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/erp_core/erp_core.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.110777 mne-1.4.1/mne/datasets/eyelink/
--rw-r--r--   0 larsoner   (501) staff       (20)       73 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/eyelink/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      748 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/eyelink/eyelink.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.111317 mne-1.4.1/mne/datasets/fieldtrip_cmc/
--rw-r--r--   0 larsoner   (501) staff       (20)      109 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/fieldtrip_cmc/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      852 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/fieldtrip_cmc/fieldtrip_cmc.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.111685 mne-1.4.1/mne/datasets/fnirs_motor/
--rw-r--r--   0 larsoner   (501) staff       (20)       76 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/fnirs_motor/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      769 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/fnirs_motor/fnirs_motor.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.112092 mne-1.4.1/mne/datasets/hf_sef/
--rw-r--r--   0 larsoner   (501) staff       (20)       53 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/hf_sef/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2867 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/hf_sef/hf_sef.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.112477 mne-1.4.1/mne/datasets/kiloword/
--rw-r--r--   0 larsoner   (501) staff       (20)       86 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/kiloword/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1989 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/kiloword/kiloword.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.112842 mne-1.4.1/mne/datasets/limo/
--rw-r--r--   0 larsoner   (501) staff       (20)       60 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/limo/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13058 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/limo/limo.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.113217 mne-1.4.1/mne/datasets/misc/
--rw-r--r--   0 larsoner   (501) staff       (20)       68 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/misc/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      851 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/misc/_misc.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.113570 mne-1.4.1/mne/datasets/mtrf/
--rw-r--r--   0 larsoner   (501) staff       (20)       62 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/mtrf/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      765 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/mtrf/mtrf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.113937 mne-1.4.1/mne/datasets/multimodal/
--rw-r--r--   0 larsoner   (501) staff       (20)       74 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/multimodal/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      879 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/multimodal/multimodal.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.114540 mne-1.4.1/mne/datasets/opm/
--rw-r--r--   0 larsoner   (501) staff       (20)       60 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/opm/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      839 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/opm/opm.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.114830 mne-1.4.1/mne/datasets/phantom_4dbti/
--rw-r--r--   0 larsoner   (501) staff       (20)       77 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/phantom_4dbti/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      792 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/phantom_4dbti/phantom_4dbti.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.115124 mne-1.4.1/mne/datasets/refmeg_noise/
--rw-r--r--   0 larsoner   (501) staff       (20)       86 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/refmeg_noise/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      770 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/refmeg_noise/refmeg_noise.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.115395 mne-1.4.1/mne/datasets/sample/
--rw-r--r--   0 larsoner   (501) staff       (20)       70 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/sample/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      859 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/sample/sample.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.116800 mne-1.4.1/mne/datasets/sleep_physionet/
--rw-r--r--   0 larsoner   (501) staff       (20)    24428 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/sleep_physionet/SHA1SUMS
--rw-r--r--   0 larsoner   (501) staff       (20)       37 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/sleep_physionet/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8092 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/sleep_physionet/_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5127 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/sleep_physionet/age.py
--rw-r--r--   0 larsoner   (501) staff       (20)    27887 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/sleep_physionet/age_records.csv
--rw-r--r--   0 larsoner   (501) staff       (20)     3772 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/sleep_physionet/temazepam.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6990 2022-11-28 17:38:12.000000 mne-1.4.1/mne/datasets/sleep_physionet/temazepam_records.csv
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.116962 mne-1.4.1/mne/datasets/sleep_physionet/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     7287 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/sleep_physionet/tests/test_physionet.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.117354 mne-1.4.1/mne/datasets/somato/
--rw-r--r--   0 larsoner   (501) staff       (20)       73 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/somato/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      859 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/somato/somato.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.117752 mne-1.4.1/mne/datasets/spm_face/
--rw-r--r--   0 larsoner   (501) staff       (20)      103 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/spm_face/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1203 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/spm_face/spm_data.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.118056 mne-1.4.1/mne/datasets/ssvep/
--rw-r--r--   0 larsoner   (501) staff       (20)       64 2022-11-28 17:38:21.000000 mne-1.4.1/mne/datasets/ssvep/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      732 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/ssvep/ssvep.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.118327 mne-1.4.1/mne/datasets/testing/
--rw-r--r--   0 larsoner   (501) staff       (20)      150 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/testing/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2119 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/testing/_testing.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.118589 mne-1.4.1/mne/datasets/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12452 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/tests/test_datasets.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.118989 mne-1.4.1/mne/datasets/ucl_opm_auditory/
--rw-r--r--   0 larsoner   (501) staff       (20)       81 2023-04-24 01:19:07.000000 mne-1.4.1/mne/datasets/ucl_opm_auditory/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      800 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/ucl_opm_auditory/ucl_opm_auditory.py
--rw-r--r--   0 larsoner   (501) staff       (20)    28071 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/utils.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.119303 mne-1.4.1/mne/datasets/visual_92_categories/
--rw-r--r--   0 larsoner   (501) staff       (20)       98 2022-05-20 17:14:56.000000 mne-1.4.1/mne/datasets/visual_92_categories/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2182 2023-06-05 14:01:41.000000 mne-1.4.1/mne/datasets/visual_92_categories/visual_92_categories.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.121816 mne-1.4.1/mne/decoding/
--rw-r--r--   0 larsoner   (501) staff       (20)      624 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19127 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/base.py
--rw-r--r--   0 larsoner   (501) staff       (20)    29368 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/csp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7623 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/ems.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2863 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/mixin.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19219 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/receptive_field.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26793 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/search_light.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14734 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/ssd.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.123427 mne-1.4.1/mne/decoding/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/decoding/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15649 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_base.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13441 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_csp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3134 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_ems.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22450 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_receptive_field.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10791 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_search_light.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13993 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_ssd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1351 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9655 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/tests/test_transformer.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13577 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/time_delaying_ridge.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5130 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)    29890 2023-06-05 14:01:41.000000 mne-1.4.1/mne/decoding/transformer.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9083 2023-06-05 14:01:41.000000 mne-1.4.1/mne/defaults.py
--rw-r--r--   0 larsoner   (501) staff       (20)    59776 2023-06-05 14:01:41.000000 mne-1.4.1/mne/dipole.py
--rw-r--r--   0 larsoner   (501) staff       (20)   156962 2023-06-05 14:01:41.000000 mne-1.4.1/mne/epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)    58244 2023-06-05 16:25:38.000000 mne-1.4.1/mne/event.py
--rw-r--r--   0 larsoner   (501) staff       (20)    63030 2023-06-05 14:01:41.000000 mne-1.4.1/mne/evoked.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.124584 mne-1.4.1/mne/export/
--rw-r--r--   0 larsoner   (501) staff       (20)      103 2022-11-28 17:38:21.000000 mne-1.4.1/mne/export/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      472 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/_brainvision.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12063 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/_edf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2510 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/_eeglab.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5620 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/_egimff.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6010 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/_export.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.124711 mne-1.4.1/mne/export/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)    19429 2023-06-05 14:01:41.000000 mne-1.4.1/mne/export/tests/test_export.py
--rw-r--r--   0 larsoner   (501) staff       (20)    95360 2023-06-05 14:01:41.000000 mne-1.4.1/mne/filter.py
--rw-r--r--   0 larsoner   (501) staff       (20)    31217 2023-06-05 14:01:41.000000 mne-1.4.1/mne/fixes.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.126044 mne-1.4.1/mne/forward/
--rw-r--r--   0 larsoner   (501) staff       (20)     1123 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    34441 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/_compute_forward.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18408 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/_field_interpolation.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19463 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/_lead_dots.py
--rw-r--r--   0 larsoner   (501) staff       (20)    31718 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/_make_forward.py
--rw-r--r--   0 larsoner   (501) staff       (20)    77927 2023-06-05 16:25:38.000000 mne-1.4.1/mne/forward/forward.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.126916 mne-1.4.1/mne/forward/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/forward/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11446 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/tests/test_field_interpolation.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18572 2023-06-05 16:25:38.000000 mne-1.4.1/mne/forward/tests/test_forward.py
--rw-r--r--   0 larsoner   (501) staff       (20)    30292 2023-06-05 14:01:41.000000 mne-1.4.1/mne/forward/tests/test_make_forward.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.127737 mne-1.4.1/mne/gui/
--rw-r--r--   0 larsoner   (501) staff       (20)    12864 2023-06-05 16:25:38.000000 mne-1.4.1/mne/gui/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    23226 2023-06-05 16:25:38.000000 mne-1.4.1/mne/gui/_core.py
--rw-r--r--   0 larsoner   (501) staff       (20)    76082 2023-06-05 14:01:41.000000 mne-1.4.1/mne/gui/_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    33695 2023-06-05 16:25:38.000000 mne-1.4.1/mne/gui/_ieeg_locate.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.128556 mne-1.4.1/mne/gui/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/gui/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2273 2023-06-05 16:25:38.000000 mne-1.4.1/mne/gui/tests/test_core.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12760 2023-06-05 14:01:41.000000 mne-1.4.1/mne/gui/tests/test_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11178 2023-06-05 14:01:41.000000 mne-1.4.1/mne/gui/tests/test_gui_api.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8479 2023-06-05 16:25:38.000000 mne-1.4.1/mne/gui/tests/test_ieeg_locate.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.129367 mne-1.4.1/mne/html/
--rw-r--r--   0 larsoner   (501) staff       (20)   146814 2022-05-20 17:14:56.000000 mne-1.4.1/mne/html/d3.v3.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)    36228 2022-05-20 17:14:56.000000 mne-1.4.1/mne/html/mpld3.v0.2.min.js
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.129776 mne-1.4.1/mne/html_templates/
--rw-r--r--   0 larsoner   (501) staff       (20)       95 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      509 2023-06-05 14:01:41.000000 mne-1.4.1/mne/html_templates/_templates.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.131769 mne-1.4.1/mne/html_templates/report/
--rw-r--r--   0 larsoner   (501) staff       (20)      217 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/bem.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      172 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/code.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      287 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/footer.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      132 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/forward.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)     1864 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/header.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      892 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/html.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      535 2023-06-05 14:01:41.000000 mne-1.4.1/mne/html_templates/report/image.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      128 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/inverse.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      993 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/section.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)     2812 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/slider.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      610 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/report/toc.html.jinja
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.133093 mne-1.4.1/mne/html_templates/repr/
--rw-r--r--   0 larsoner   (501) staff       (20)      599 2023-06-05 14:01:41.000000 mne-1.4.1/mne/html_templates/repr/epochs.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      689 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/evoked.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      449 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/forward.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      811 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/ica.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)     1836 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/info.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      354 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/inverse_operator.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)      256 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/raw.html.jinja
--rw-r--r--   0 larsoner   (501) staff       (20)     1329 2022-11-28 17:38:21.000000 mne-1.4.1/mne/html_templates/repr/spectrum.html.jinja
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.135108 mne-1.4.1/mne/icons/
--rw-r--r--   0 larsoner   (501) staff       (20)      290 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/README.rst
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.135290 mne-1.4.1/mne/icons/dark/
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.137331 mne-1.4.1/mne/icons/dark/actions/
--rw-r--r--   0 larsoner   (501) staff       (20)      252 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/clear.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      276 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/folder.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      402 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/help.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      442 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/movie.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      452 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/pause.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      405 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/play.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      372 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/reset.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      377 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/restore.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      685 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/scale.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      396 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/screenshot.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      901 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/visibility_off.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      493 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/actions/visibility_on.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      116 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/dark/index.theme
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.137496 mne-1.4.1/mne/icons/light/
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.139733 mne-1.4.1/mne/icons/light/actions/
--rw-r--r--   0 larsoner   (501) staff       (20)      252 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/clear.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      276 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/folder.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      402 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/help.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      442 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/movie.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      452 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/pause.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      405 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/play.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      372 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/reset.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      377 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/restore.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      685 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/scale.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      396 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/screenshot.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      901 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/visibility_off.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      493 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/actions/visibility_on.svg
--rw-r--r--   0 larsoner   (501) staff       (20)      117 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/light/index.theme
--rw-r--r--   0 larsoner   (501) staff       (20)    44028 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/mne_bigsur_icon.png
--rw-r--r--   0 larsoner   (501) staff       (20)    10369 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/mne_default_icon.png
--rw-r--r--   0 larsoner   (501) staff       (20)    44818 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/mne_icon-cropped.png
--rw-r--r--   0 larsoner   (501) staff       (20)    31258 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/mne_icon.png
--rw-r--r--   0 larsoner   (501) staff       (20)    22283 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/mne_splash.png
--rw-r--r--   0 larsoner   (501) staff       (20)      304 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/toolbar_move_horizontal@2x.png
--rw-r--r--   0 larsoner   (501) staff       (20)      208 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/toolbar_move_vertical@2x.png
--rw-r--r--   0 larsoner   (501) staff       (20)      151 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/toolbar_separator_horizontal.png
--rw-r--r--   0 larsoner   (501) staff       (20)      288 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/toolbar_separator_horizontal@2x.png
--rw-r--r--   0 larsoner   (501) staff       (20)      192 2022-11-28 17:38:21.000000 mne-1.4.1/mne/icons/toolbar_separator_vertical@2x.png
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.140693 mne-1.4.1/mne/inverse_sparse/
--rw-r--r--   0 larsoner   (501) staff       (20)      239 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10212 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/_gamma_map.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3564 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/mxne_debiasing.py
--rw-r--r--   0 larsoner   (501) staff       (20)    35158 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/mxne_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)    54504 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/mxne_optim.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.141792 mne-1.4.1/mne/inverse_sparse/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/inverse_sparse/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6754 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/tests/test_gamma_map.py
--rw-r--r--   0 larsoner   (501) staff       (20)      807 2022-11-28 17:38:21.000000 mne-1.4.1/mne/inverse_sparse/tests/test_mxne_debiasing.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19290 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/tests/test_mxne_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14735 2023-06-05 14:01:41.000000 mne-1.4.1/mne/inverse_sparse/tests/test_mxne_optim.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.148179 mne-1.4.1/mne/io/
--rw-r--r--   0 larsoner   (501) staff       (20)     2231 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20833 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/_digitization.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4589 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/_read_raw.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.148586 mne-1.4.1/mne/io/array/
--rw-r--r--   0 larsoner   (501) staff       (20)      120 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/array/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3234 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/array/array.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.148911 mne-1.4.1/mne/io/array/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/array/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6725 2023-06-05 16:25:38.000000 mne-1.4.1/mne/io/array/tests/test_array.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.149740 mne-1.4.1/mne/io/artemis123/
--rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/artemis123/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19620 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/artemis123/artemis123.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.150255 mne-1.4.1/mne/io/artemis123/resources/
--rw-r--r--   0 larsoner   (501) staff       (20)     9272 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/artemis123/resources/Artemis123_ChannelMap.csv
--rw-r--r--   0 larsoner   (501) staff       (20)    25854 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/artemis123/resources/Artemis123_mneLoc.csv
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.150768 mne-1.4.1/mne/io/artemis123/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/artemis123/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4407 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/artemis123/tests/test_artemis123.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4365 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/artemis123/utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)   105890 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/base.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.151120 mne-1.4.1/mne/io/besa/
--rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/besa/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8977 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/besa/besa.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.151373 mne-1.4.1/mne/io/besa/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     2890 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/besa/tests/test_besa.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.151886 mne-1.4.1/mne/io/boxy/
--rw-r--r--   0 larsoner   (501) staff       (20)      166 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/boxy/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11481 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/boxy/boxy.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.152120 mne-1.4.1/mne/io/boxy/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/boxy/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7599 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/boxy/tests/test_boxy.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.152488 mne-1.4.1/mne/io/brainvision/
--rw-r--r--   0 larsoner   (501) staff       (20)      226 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/brainvision/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    41837 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/brainvision/brainvision.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.152854 mne-1.4.1/mne/io/brainvision/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        1 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/brainvision/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    31664 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/brainvision/tests/test_brainvision.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.154059 mne-1.4.1/mne/io/bti/
--rw-r--r--   0 larsoner   (501) staff       (20)      127 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/bti/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    52902 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/bti/bti.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2323 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/bti/constants.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2878 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/bti/read.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.154291 mne-1.4.1/mne/io/bti/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/bti/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17651 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/bti/tests/test_bti.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.154857 mne-1.4.1/mne/io/cnt/
--rw-r--r--   0 larsoner   (501) staff       (20)       54 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/cnt/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4767 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/cnt/_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22378 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/cnt/cnt.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.155159 mne-1.4.1/mne/io/cnt/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/cnt/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1973 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/cnt/tests/test_cnt.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5667 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/compensator.py
--rw-r--r--   0 larsoner   (501) staff       (20)    40164 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/constants.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.156973 mne-1.4.1/mne/io/ctf/
--rw-r--r--   0 larsoner   (501) staff       (20)      154 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/ctf/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      726 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/constants.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11047 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/ctf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3781 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/eeg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2492 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/hc.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20449 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/info.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2865 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/markers.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7078 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/res4.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.157209 mne-1.4.1/mne/io/ctf/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/ctf/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    24782 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/tests/test_ctf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4778 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf/trans.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5884 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/ctf_comp.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.157673 mne-1.4.1/mne/io/curry/
--rw-r--r--   0 larsoner   (501) staff       (20)      144 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/curry/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21398 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/curry/curry.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.157962 mne-1.4.1/mne/io/curry/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.1/mne/io/curry/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18899 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/curry/tests/test_curry.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1217 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/diff.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.158360 mne-1.4.1/mne/io/edf/
--rw-r--r--   0 larsoner   (501) staff       (20)      177 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/edf/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    71710 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/edf/edf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.159448 mne-1.4.1/mne/io/edf/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/edf/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    28995 2023-06-05 16:25:38.000000 mne-1.4.1/mne/io/edf/tests/test_edf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5920 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/edf/tests/test_gdf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.160003 mne-1.4.1/mne/io/eeglab/
--rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:12.000000 mne-1.4.1/mne/io/eeglab/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2496 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eeglab/_eeglab.py
--rw-r--r--   0 larsoner   (501) staff       (20)    27991 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eeglab/eeglab.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.160344 mne-1.4.1/mne/io/eeglab/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/eeglab/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22820 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eeglab/tests/test_eeglab.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.161282 mne-1.4.1/mne/io/egi/
--rw-r--r--   0 larsoner   (501) staff       (20)      164 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/egi/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11929 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/egi/egi.py
--rw-r--r--   0 larsoner   (501) staff       (20)    40256 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/egi/egimff.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4726 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/egi/events.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6230 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/egi/general.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.161530 mne-1.4.1/mne/io/egi/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/egi/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19662 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/egi/tests/test_egi.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.161939 mne-1.4.1/mne/io/eximia/
--rw-r--r--   0 larsoner   (501) staff       (20)      155 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/eximia/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3185 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eximia/eximia.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.162380 mne-1.4.1/mne/io/eximia/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/eximia/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1622 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eximia/tests/test_eximia.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.162788 mne-1.4.1/mne/io/eyelink/
--rw-r--r--   0 larsoner   (501) staff       (20)      156 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eyelink/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    36953 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eyelink/eyelink.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.163105 mne-1.4.1/mne/io/eyelink/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eyelink/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6246 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/eyelink/tests/test_eyelink.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.163548 mne-1.4.1/mne/io/fieldtrip/
--rw-r--r--   0 larsoner   (501) staff       (20)      247 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fieldtrip/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6673 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fieldtrip/fieldtrip.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.163994 mne-1.4.1/mne/io/fieldtrip/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)      158 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/fieldtrip/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6446 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fieldtrip/tests/helpers.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12151 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fieldtrip/tests/test_fieldtrip.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12204 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fieldtrip/utils.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.164350 mne-1.4.1/mne/io/fiff/
--rw-r--r--   0 larsoner   (501) staff       (20)       79 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/fiff/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20787 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fiff/raw.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.164614 mne-1.4.1/mne/io/fiff/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/fiff/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    77607 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fiff/tests/test_raw_fiff.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.165148 mne-1.4.1/mne/io/fil/
--rw-r--r--   0 larsoner   (501) staff       (20)      105 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fil/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10467 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fil/fil.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4501 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fil/sensors.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.165295 mne-1.4.1/mne/io/fil/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     4270 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/fil/tests/test_fil.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.165597 mne-1.4.1/mne/io/hitachi/
--rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/hitachi/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12655 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/hitachi/hitachi.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.165733 mne-1.4.1/mne/io/hitachi/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)    59466 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/hitachi/tests/test_hitachi.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.166467 mne-1.4.1/mne/io/kit/
--rw-r--r--   0 larsoner   (501) staff       (20)      188 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/kit/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9156 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/constants.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7774 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    36969 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/kit.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.166970 mne-1.4.1/mne/io/kit/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)       68 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      984 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/tests/test_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16867 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/kit/tests/test_kit.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4398 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/matrix.py
--rw-r--r--   0 larsoner   (501) staff       (20)   114631 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/meas_info.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.167886 mne-1.4.1/mne/io/nedf/
--rw-r--r--   0 larsoner   (501) staff       (20)      162 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/nedf/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7783 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nedf/nedf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.168303 mne-1.4.1/mne/io/nedf/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        1 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/nedf/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4467 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nedf/tests/test_nedf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.168678 mne-1.4.1/mne/io/nicolet/
--rw-r--r--   0 larsoner   (501) staff       (20)      165 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/nicolet/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6568 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nicolet/nicolet.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.168916 mne-1.4.1/mne/io/nicolet/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.1/mne/io/nicolet/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      750 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nicolet/tests/test_nicolet.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.169206 mne-1.4.1/mne/io/nihon/
--rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/nihon/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18051 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nihon/nihon.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.169385 mne-1.4.1/mne/io/nihon/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     3453 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nihon/tests/test_nihon.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.169880 mne-1.4.1/mne/io/nirx/
--rw-r--r--   0 larsoner   (501) staff       (20)      146 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/nirx/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3950 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nirx/_localized_abbr.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22266 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nirx/nirx.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.170155 mne-1.4.1/mne/io/nirx/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.1/mne/io/nirx/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26253 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/nirx/tests/test_nirx.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11246 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/open.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.170633 mne-1.4.1/mne/io/persyst/
--rw-r--r--   0 larsoner   (501) staff       (20)      149 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/persyst/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16850 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/persyst/persyst.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.170936 mne-1.4.1/mne/io/persyst/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/persyst/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8750 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/persyst/tests/test_persyst.py
--rw-r--r--   0 larsoner   (501) staff       (20)    46005 2023-06-05 16:25:38.000000 mne-1.4.1/mne/io/pick.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11702 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/proc_history.py
--rw-r--r--   0 larsoner   (501) staff       (20)    38454 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/proj.py
--rw-r--r--   0 larsoner   (501) staff       (20)    24159 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/reference.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.171253 mne-1.4.1/mne/io/snirf/
--rw-r--r--   0 larsoner   (501) staff       (20)      149 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/snirf/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22347 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/snirf/_snirf.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.171543 mne-1.4.1/mne/io/snirf/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.1/mne/io/snirf/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15517 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/snirf/tests/test_snirf.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18102 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tag.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.174062 mne-1.4.1/mne/io/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)       71 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1892 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_apply_function.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4249 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_compensator.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14879 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_constants.py
--rw-r--r--   0 larsoner   (501) staff       (20)    40085 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_meas_info.py
--rw-r--r--   0 larsoner   (501) staff       (20)    28743 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_pick.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1403 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_proc_history.py
--rw-r--r--   0 larsoner   (501) staff       (20)    36373 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2891 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_read_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)    32089 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_reference.py
--rw-r--r--   0 larsoner   (501) staff       (20)      917 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_show_fiff.py
--rw-r--r--   0 larsoner   (501) staff       (20)      578 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1720 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_what.py
--rw-r--r--   0 larsoner   (501) staff       (20)      782 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tests/test_write.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4694 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/tree.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11601 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2128 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/what.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17887 2023-06-05 14:01:41.000000 mne-1.4.1/mne/io/write.py
--rw-r--r--   0 larsoner   (501) staff       (20)   100868 2023-06-05 14:01:41.000000 mne-1.4.1/mne/label.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.175140 mne-1.4.1/mne/minimum_norm/
--rw-r--r--   0 larsoner   (501) staff       (20)      724 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7301 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/_eloreta.py
--rw-r--r--   0 larsoner   (501) staff       (20)    72953 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16454 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/resolution_matrix.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12826 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/spatial_resolution.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.176350 mne-1.4.1/mne/minimum_norm/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/minimum_norm/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    62883 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/tests/test_inverse.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9806 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/tests/test_resolution_matrix.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5905 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/tests/test_resolution_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1514 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/tests/test_snr.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8495 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/tests/test_time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)    30779 2023-06-05 14:01:41.000000 mne-1.4.1/mne/minimum_norm/time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2926 2023-06-05 14:01:41.000000 mne-1.4.1/mne/misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)    58424 2023-06-05 14:01:41.000000 mne-1.4.1/mne/morph.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9169 2023-06-05 14:01:41.000000 mne-1.4.1/mne/morph_map.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4848 2023-06-05 14:01:41.000000 mne-1.4.1/mne/parallel.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.180732 mne-1.4.1/mne/preprocessing/
--rw-r--r--   0 larsoner   (501) staff       (20)     1716 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11302 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/_csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2963 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/_css.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20851 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/_fine_cal.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6277 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/_peak_finder.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13215 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/_regress.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11365 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/annotate_amplitude.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1139 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/annotate_nan.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22725 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/artifact_detection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1549 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/bads.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5139 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ctps_.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15571 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ecg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9572 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/eog.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.181307 mne-1.4.1/mne/preprocessing/eyetracking/
--rw-r--r--   0 larsoner   (501) staff       (20)      186 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/eyetracking/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5475 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/eyetracking/eyetracking.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3368 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/hfc.py
--rw-r--r--   0 larsoner   (501) staff       (20)   127544 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ica.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.181811 mne-1.4.1/mne/preprocessing/ieeg/
--rw-r--r--   0 larsoner   (501) staff       (20)      242 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ieeg/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7434 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ieeg/_projection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8858 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ieeg/_volume.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.182128 mne-1.4.1/mne/preprocessing/ieeg/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     7620 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ieeg/tests/test_projection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4713 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ieeg/tests/test_volume.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11695 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/infomax_.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8651 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/interpolate.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6448 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/maxfilter.py
--rw-r--r--   0 larsoner   (501) staff       (20)   111776 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/maxwell.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.183084 mne-1.4.1/mne/preprocessing/nirs/
--rw-r--r--   0 larsoner   (501) staff       (20)      711 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3697 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/_beer_lambert_law.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1719 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/_optical_density.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1861 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/_scalp_coupling_index.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5020 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/_tddr.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11536 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/nirs.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.184002 mne-1.4.1/mne/preprocessing/nirs/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     3525 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/tests/test_beer_lambert_law.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20195 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/tests/test_nirs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1991 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/tests/test_optical_density.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2579 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/tests/test_scalp_coupling_index.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1989 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/nirs/tests/test_temporal_derivative_distribution_repair.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5040 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/otp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4251 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/realign.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15699 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/ssp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4375 2023-06-05 16:25:38.000000 mne-1.4.1/mne/preprocessing/stim.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.188063 mne-1.4.1/mne/preprocessing/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/preprocessing/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16015 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_annotate_amplitude.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1554 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_annotate_nan.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9840 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_artifact_detection.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8921 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1697 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_css.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2914 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_ctps.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3481 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_ecg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6953 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_eeglab_infomax.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1103 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_eog.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6236 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_fine_cal.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5495 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_hfc.py
--rw-r--r--   0 larsoner   (501) staff       (20)    61957 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_ica.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6022 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_infomax.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7517 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_interpolate.py
--rw-r--r--   0 larsoner   (501) staff       (20)    71419 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_maxwell.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3770 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_otp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1168 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_peak_finder.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5050 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_realign.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6864 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_regress.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9007 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_ssp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4074 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_stim.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12753 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/tests/test_xdawn.py
--rw-r--r--   0 larsoner   (501) staff       (20)    24815 2023-06-05 14:01:41.000000 mne-1.4.1/mne/preprocessing/xdawn.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16185 2023-06-05 16:25:38.000000 mne-1.4.1/mne/proj.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17313 2023-06-05 14:01:41.000000 mne-1.4.1/mne/rank.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.188548 mne-1.4.1/mne/report/
--rw-r--r--   0 larsoner   (501) staff       (20)       56 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/__init__.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.191191 mne-1.4.1/mne/report/js_and_css/
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.192441 mne-1.4.1/mne/report/js_and_css/bootstrap-icons/
--rw-r--r--   0 larsoner   (501) staff       (20)   186639 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-icons/bootstrap-icons.mne.min.css
--rw-r--r--   0 larsoner   (501) staff       (20)     1483 2023-06-05 14:01:41.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-icons/gen_css_for_mne.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.193816 mne-1.4.1/mne/report/js_and_css/bootstrap-table/
--rw-r--r--   0 larsoner   (501) staff       (20)    15127 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table-copy-rows.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)    28095 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table-export.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)     9246 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.css
--rw-r--r--   0 larsoner   (501) staff       (20)   121976 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)    77394 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap-table/tableExport.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)    78871 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap.bundle.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)   162764 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/bootstrap.min.css
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.194526 mne-1.4.1/mne/report/js_and_css/highlightjs/
--rw-r--r--   0 larsoner   (501) staff       (20)     1193 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/highlightjs/atom-one-dark-reasonable.min.css
--rw-r--r--   0 larsoner   (501) staff       (20)      856 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/highlightjs/atom-one-light.min.css
--rw-r--r--   0 larsoner   (501) staff       (20)     1147 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/highlightjs/default.min.css
--rw-r--r--   0 larsoner   (501) staff       (20)   132027 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/highlightjs/highlight.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)    89501 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/jquery-3.6.0.min.js
--rw-r--r--   0 larsoner   (501) staff       (20)     8008 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/report.js
--rw-r--r--   0 larsoner   (501) staff       (20)      257 2022-11-28 17:38:21.000000 mne-1.4.1/mne/report/js_and_css/report.sass
--rw-r--r--   0 larsoner   (501) staff       (20)   143136 2023-06-05 16:25:38.000000 mne-1.4.1/mne/report/report.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.194849 mne-1.4.1/mne/report/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)    38595 2023-06-05 14:01:41.000000 mne-1.4.1/mne/report/tests/test_report.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.196001 mne-1.4.1/mne/simulation/
--rw-r--r--   0 larsoner   (501) staff       (20)      270 2023-04-21 22:27:15.000000 mne-1.4.1/mne/simulation/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)      419 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5498 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/evoked.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.196329 mne-1.4.1/mne/simulation/metrics/
--rw-r--r--   0 larsoner   (501) staff       (20)      348 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/metrics/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17520 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/metrics/metrics.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.196623 mne-1.4.1/mne/simulation/metrics/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.1/mne/simulation/metrics/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9371 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/metrics/tests/test_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)    30788 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21249 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/source.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.197354 mne-1.4.1/mne/simulation/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/simulation/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7263 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/tests/test_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1782 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/tests/test_metrics.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22779 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/tests/test_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15089 2023-06-05 14:01:41.000000 mne-1.4.1/mne/simulation/tests/test_source.py
--rw-r--r--   0 larsoner   (501) staff       (20)   131857 2023-06-05 14:01:41.000000 mne-1.4.1/mne/source_estimate.py
--rw-r--r--   0 larsoner   (501) staff       (20)   121184 2023-06-05 14:01:41.000000 mne-1.4.1/mne/source_space.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.198778 mne-1.4.1/mne/stats/
--rw-r--r--   0 larsoner   (501) staff       (20)      662 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4702 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/_adjacency.py
--rw-r--r--   0 larsoner   (501) staff       (20)    60183 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/cluster_level.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2997 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/multi_comp.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14482 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/parametric.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6035 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/permutations.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17689 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/regression.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.199905 mne-1.4.1/mne/stats/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/stats/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1309 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/tests/test_adjacency.py
--rw-r--r--   0 larsoner   (501) staff       (20)    30632 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/tests/test_cluster_level.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1952 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/tests/test_multi_comp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5963 2023-06-05 14:01:41.000000 mne-1.4.1/mne/stats/tests/test_parametric.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2760 2023-06-05 16:25:38.000000 mne-1.4.1/mne/stats/tests/test_permutations.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5558 2023-06-05 16:25:38.000000 mne-1.4.1/mne/stats/tests/test_regression.py
--rw-r--r--   0 larsoner   (501) staff       (20)    80420 2023-06-05 16:25:38.000000 mne-1.4.1/mne/surface.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.206839 mne-1.4.1/mne/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.1/mne/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    65393 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_annotations.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22891 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_bem.py
--rw-r--r--   0 larsoner   (501) staff       (20)    31426 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_chpi.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22434 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    35365 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_cov.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1952 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_defaults.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21338 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_dipole.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11111 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_docstring_parameters.py
--rw-r--r--   0 larsoner   (501) staff       (20)   170384 2023-06-05 16:25:38.000000 mne-1.4.1/mne/tests/test_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)    23810 2023-06-05 16:25:38.000000 mne-1.4.1/mne/tests/test_event.py
--rw-r--r--   0 larsoner   (501) staff       (20)    35726 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)    36094 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_filter.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10356 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_freesurfer.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1864 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_import_nesting.py
--rw-r--r--   0 larsoner   (501) staff       (20)    43386 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_label.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2778 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_line_endings.py
--rw-r--r--   0 larsoner   (501) staff       (20)      362 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)    43508 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_morph.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2165 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_morph_map.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4672 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_ola.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1121 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_parallel.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21664 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_proj.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11588 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_rank.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1953 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_read_vectorview_selection.py
--rw-r--r--   0 larsoner   (501) staff       (20)    75965 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_source_estimate.py
--rw-r--r--   0 larsoner   (501) staff       (20)    39370 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_source_space.py
--rw-r--r--   0 larsoner   (501) staff       (20)    19680 2023-06-05 16:25:38.000000 mne-1.4.1/mne/tests/test_surface.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22045 2023-06-05 14:01:41.000000 mne-1.4.1/mne/tests/test_transforms.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.208838 mne-1.4.1/mne/time_frequency/
--rw-r--r--   0 larsoner   (501) staff       (20)      746 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6811 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/_stft.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9665 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/_stockwell.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2335 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/ar.py
--rw-r--r--   0 larsoner   (501) staff       (20)    50272 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17488 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/multitaper.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7629 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/psd.py
--rw-r--r--   0 larsoner   (501) staff       (20)    47024 2023-06-05 16:25:38.000000 mne-1.4.1/mne/time_frequency/spectrum.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.210726 mne-1.4.1/mne/time_frequency/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/time_frequency/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1805 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_ar.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21280 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_csd.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2943 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_multitaper.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8129 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_psd.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12507 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_spectrum.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2204 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_stft.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5365 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_stockwell.py
--rw-r--r--   0 larsoner   (501) staff       (20)    50185 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tests/test_tfr.py
--rw-r--r--   0 larsoner   (501) staff       (20)   110913 2023-06-05 14:01:41.000000 mne-1.4.1/mne/time_frequency/tfr.py
--rw-r--r--   0 larsoner   (501) staff       (20)    66973 2023-06-05 14:01:41.000000 mne-1.4.1/mne/transforms.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.215215 mne-1.4.1/mne/utils/
--rw-r--r--   0 larsoner   (501) staff       (20)     4443 2023-06-05 16:25:38.000000 mne-1.4.1/mne/utils/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3035 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/_bunch.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17017 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/_logging.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13569 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/_testing.py
--rw-r--r--   0 larsoner   (501) staff       (20)    40479 2023-06-05 16:25:38.000000 mne-1.4.1/mne/utils/check.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26682 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/config.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3772 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/dataframe.py
--rw-r--r--   0 larsoner   (501) staff       (20)   174485 2023-06-05 16:25:38.000000 mne-1.4.1/mne/utils/docs.py
--rw-r--r--   0 larsoner   (501) staff       (20)      583 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/fetching.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6450 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/linalg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15198 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26420 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/mixin.py
--rw-r--r--   0 larsoner   (501) staff       (20)    38080 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/numerics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6724 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/progressbar.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2732 2023-06-05 16:25:38.000000 mne-1.4.1/mne/utils/spectrum.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.217085 mne-1.4.1/mne/utils/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)      643 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_bunch.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11942 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_check.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4679 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_config.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5783 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_docs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3668 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_linalg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8439 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_logging.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4102 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.1/mne/utils/tests/test_mixin.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21290 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_numerics.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4324 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_progressbar.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1569 2023-06-05 14:01:41.000000 mne-1.4.1/mne/utils/tests/test_testing.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.224341 mne-1.4.1/mne/viz/
--rw-r--r--   0 larsoner   (501) staff       (20)   144063 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_3d.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5679 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_3d_overlay.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2141 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/__init__.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.226994 mne-1.4.1/mne/viz/_brain/
--rw-r--r--   0 larsoner   (501) staff       (20)      510 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)   156784 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/_brain.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5432 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/_linkviewer.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4034 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/_scraper.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3714 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/callback.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6463 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/colormap.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6322 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/surface.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.227314 mne-1.4.1/mne/viz/_brain/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)    46475 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/tests/test_brain.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5542 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/tests/test_notebook.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2455 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_brain/view.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7020 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_dipole.py
--rw-r--r--   0 larsoner   (501) staff       (20)    31796 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_figure.py
--rw-r--r--   0 larsoner   (501) staff       (20)   105679 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_mpl_figure.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9716 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_proj.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2687 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/_scraper.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.229839 mne-1.4.1/mne/viz/backends/
--rw-r--r--   0 larsoner   (501) staff       (20)       53 2022-11-28 17:38:12.000000 mne-1.4.1/mne/viz/backends/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    37818 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/_abstract.py
--rw-r--r--   0 larsoner   (501) staff       (20)    50094 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/_notebook.py
--rw-r--r--   0 larsoner   (501) staff       (20)    46923 2023-06-05 16:24:17.000000 mne-1.4.1/mne/viz/backends/_pyvista.py
--rw-r--r--   0 larsoner   (501) staff       (20)    59516 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/_qt.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15557 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11950 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/renderer.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.230435 mne-1.4.1/mne/viz/backends/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)     1164 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/tests/_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4553 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/tests/test_abstract.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7437 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/tests/test_renderer.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3869 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/backends/tests/test_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15169 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/circle.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1633 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/conftest.py
--rw-r--r--   0 larsoner   (501) staff       (20)    42586 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)   117627 2023-06-05 16:25:38.000000 mne-1.4.1/mne/viz/evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)    44556 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/ica.py
--rw-r--r--   0 larsoner   (501) staff       (20)    54351 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2847 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/montage.py
--rw-r--r--   0 larsoner   (501) staff       (20)    20840 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/raw.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.233943 mne-1.4.1/mne/viz/tests/
--rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.1/mne/viz/tests/__init__.py
--rw-r--r--   0 larsoner   (501) staff       (20)    38878 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_3d.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5336 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_3d_mpl.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1054 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_circle.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18499 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)    23911 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)      366 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_figure.py
--rw-r--r--   0 larsoner   (501) staff       (20)    17568 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_ica.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11878 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_misc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2757 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_montage.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2235 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_proj.py
--rw-r--r--   0 larsoner   (501) staff       (20)    41544 2023-06-05 16:25:38.000000 mne-1.4.1/mne/viz/tests/test_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     1003 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_scraper.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13267 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_topo.py
--rw-r--r--   0 larsoner   (501) staff       (20)    33336 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_topomap.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6990 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/tests/test_utils.py
--rw-r--r--   0 larsoner   (501) staff       (20)    40149 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/topo.py
--rw-r--r--   0 larsoner   (501) staff       (20)   126112 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/topomap.py
--rw-r--r--   0 larsoner   (501) staff       (20)    99194 2023-06-05 14:01:41.000000 mne-1.4.1/mne/viz/utils.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.065361 mne-1.4.1/mne.egg-info/
--rw-r--r--   0 larsoner   (501) staff       (20)     6944 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/PKG-INFO
--rw-r--r--   0 larsoner   (501) staff       (20)    36048 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/SOURCES.txt
--rw-r--r--   0 larsoner   (501) staff       (20)        1 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/dependency_links.txt
--rw-r--r--   0 larsoner   (501) staff       (20)       48 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/entry_points.txt
--rw-r--r--   0 larsoner   (501) staff       (20)        1 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/not-zip-safe
--rw-r--r--   0 larsoner   (501) staff       (20)      434 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/requires.txt
--rw-r--r--   0 larsoner   (501) staff       (20)        4 2023-06-05 16:28:41.000000 mne-1.4.1/mne.egg-info/top_level.txt
--rw-r--r--   0 larsoner   (501) staff       (20)     1554 2023-06-05 14:01:41.000000 mne-1.4.1/pyproject.toml
--rw-r--r--   0 larsoner   (501) staff       (20)      799 2023-06-05 16:25:38.000000 mne-1.4.1/requirements.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      188 2023-06-05 14:01:41.000000 mne-1.4.1/requirements_base.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      530 2023-06-05 14:01:41.000000 mne-1.4.1/requirements_doc.txt
--rw-r--r--   0 larsoner   (501) staff       (20)       75 2022-11-28 17:38:21.000000 mne-1.4.1/requirements_hdf5.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      223 2023-06-05 14:01:41.000000 mne-1.4.1/requirements_testing.txt
--rw-r--r--   0 larsoner   (501) staff       (20)      173 2023-06-05 14:01:41.000000 mne-1.4.1/requirements_testing_extra.txt
--rw-r--r--   0 larsoner   (501) staff       (20)       38 2023-06-05 16:28:42.252173 mne-1.4.1/setup.cfg
--rw-r--r--   0 larsoner   (501) staff       (20)     5491 2023-06-05 16:25:38.000000 mne-1.4.1/setup.py
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.234110 mne-1.4.1/tutorials/
--rw-r--r--   0 larsoner   (501) staff       (20)      856 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.234906 mne-1.4.1/tutorials/clinical/
--rw-r--r--   0 larsoner   (501) staff       (20)     8652 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/clinical/20_seeg.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7944 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/clinical/30_ecog.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11308 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/clinical/60_sleep.py
--rw-r--r--   0 larsoner   (501) staff       (20)      849 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/clinical/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.236466 mne-1.4.1/tutorials/epochs/
--rw-r--r--   0 larsoner   (501) staff       (20)    17931 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/10_epochs_overview.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11211 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/15_baseline_regression.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12231 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/20_visualize_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6895 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/30_epochs_metadata.py
--rw-r--r--   0 larsoner   (501) staff       (20)    18668 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/40_autogenerate_metadata.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6295 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/50_epochs_to_data_frame.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5100 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/epochs/60_make_fixed_length_epochs.py
--rw-r--r--   0 larsoner   (501) staff       (20)      169 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/epochs/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.237343 mne-1.4.1/tutorials/evoked/
--rw-r--r--   0 larsoner   (501) staff       (20)    15451 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/evoked/10_evoked_overview.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11855 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/evoked/20_visualize_evoked.py
--rw-r--r--   0 larsoner   (501) staff       (20)    28275 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/evoked/30_eeg_erp.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2327 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/evoked/40_whitened.py
--rw-r--r--   0 larsoner   (501) staff       (20)      183 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/evoked/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.238889 mne-1.4.1/tutorials/forward/
--rw-r--r--   0 larsoner   (501) staff       (20)     5741 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/10_background_freesurfer.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16105 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/20_source_alignment.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4183 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/25_automated_coreg.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10233 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/30_forward.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5278 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/35_eeg_no_mri.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21487 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/50_background_freesurfer_mne.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14059 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/80_fix_bem_in_blender.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7966 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/forward/90_compute_covariance.py
--rw-r--r--   0 larsoner   (501) staff       (20)      196 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/forward/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.240276 mne-1.4.1/tutorials/intro/
--rw-r--r--   0 larsoner   (501) staff       (20)    18252 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/10_overview.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4034 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/15_inplace.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13980 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/20_events_from_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7745 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/30_info.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13146 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/40_sensor_locations.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9643 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/50_configure_mne.py
--rw-r--r--   0 larsoner   (501) staff       (20)    27642 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/intro/70_report.py
--rw-r--r--   0 larsoner   (501) staff       (20)      321 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/intro/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.242311 mne-1.4.1/tutorials/inverse/
--rw-r--r--   0 larsoner   (501) staff       (20)     9293 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/10_stc_class.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4775 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/20_dipole_fit.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4895 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/30_mne_dspm_loreta.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9462 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/35_dipole_orientations.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3614 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/40_mne_fixed_free.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12118 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/50_beamformer_lcmv.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7664 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/60_visualize_stc.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6646 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/70_eeg_mri_coords.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6531 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/80_brainstorm_phantom_elekta.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3862 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/85_brainstorm_phantom_ctf.py
--rw-r--r--   0 larsoner   (501) staff       (20)     2505 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/inverse/90_phantom_4DBTi.py
--rw-r--r--   0 larsoner   (501) staff       (20)      145 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/inverse/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.243326 mne-1.4.1/tutorials/io/
--rw-r--r--   0 larsoner   (501) staff       (20)    13012 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/io/10_reading_meg_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9041 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/io/20_reading_eeg_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)    10187 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/io/30_reading_fnirs_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)    14167 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/io/60_ctf_bst_auditory.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7858 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/io/70_reading_eyetracking_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)      218 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/io/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.243929 mne-1.4.1/tutorials/machine-learning/
--rw-r--r--   0 larsoner   (501) staff       (20)    13605 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/machine-learning/30_strf.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16655 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/machine-learning/50_decoding.py
--rw-r--r--   0 larsoner   (501) staff       (20)      171 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/machine-learning/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.247088 mne-1.4.1/tutorials/preprocessing/
--rw-r--r--   0 larsoner   (501) staff       (20)    11133 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/10_preprocessing_overview.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12395 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/15_handling_bad_channels.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13749 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/20_rejecting_bad_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)    46385 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/25_background_filtering.py
--rw-r--r--   0 larsoner   (501) staff       (20)    13464 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/30_filtering_resampling.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9913 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/35_artifact_correction_regression.py
--rw-r--r--   0 larsoner   (501) staff       (20)    30001 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/40_artifact_correction_ica.py
--rw-r--r--   0 larsoner   (501) staff       (20)    21535 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/45_projectors_background.py
--rw-r--r--   0 larsoner   (501) staff       (20)    22828 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/50_artifact_correction_ssp.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11436 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/55_setting_eeg_reference.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3736 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/59_head_positions.py
--rw-r--r--   0 larsoner   (501) staff       (20)    16567 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/60_maxwell_filtering_sss.py
--rw-r--r--   0 larsoner   (501) staff       (20)    12305 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/70_fnirs_processing.py
--rw-r--r--   0 larsoner   (501) staff       (20)     8828 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/80_opm_processing.py
--rw-r--r--   0 larsoner   (501) staff       (20)     3866 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/preprocessing/90_eyetracking_data.py
--rw-r--r--   0 larsoner   (501) staff       (20)      150 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/preprocessing/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.248131 mne-1.4.1/tutorials/raw/
--rw-r--r--   0 larsoner   (501) staff       (20)       22 2022-11-28 17:38:12.000000 mne-1.4.1/tutorials/raw/.gitignore
--rw-r--r--   0 larsoner   (501) staff       (20)    25952 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/raw/10_raw_overview.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7984 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/raw/20_event_arrays.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11027 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/raw/30_annotate_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9168 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/raw/40_visualize_raw.py
--rw-r--r--   0 larsoner   (501) staff       (20)      242 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/raw/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.248693 mne-1.4.1/tutorials/simulation/
--rw-r--r--   0 larsoner   (501) staff       (20)     9124 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/simulation/10_array_objs.py
--rw-r--r--   0 larsoner   (501) staff       (20)     6182 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/simulation/70_point_spread.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11401 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/simulation/80_dics.py
--rw-r--r--   0 larsoner   (501) staff       (20)      177 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/simulation/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.249854 mne-1.4.1/tutorials/stats-sensor-space/
--rw-r--r--   0 larsoner   (501) staff       (20)    29116 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/10_background_stats.py
--rw-r--r--   0 larsoner   (501) staff       (20)     5491 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/20_erp_stats.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9511 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/40_cluster_1samp_time_freq.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4894 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/50_cluster_between_time_freq.py
--rw-r--r--   0 larsoner   (501) staff       (20)     9833 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/70_cluster_rmANOVA_time_freq.py
--rw-r--r--   0 larsoner   (501) staff       (20)    15038 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-sensor-space/75_cluster_ftest_spatiotemporal.py
--rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/stats-sensor-space/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.250841 mne-1.4.1/tutorials/stats-source-space/
--rw-r--r--   0 larsoner   (501) staff       (20)     9178 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-source-space/20_cluster_1samp_spatiotemporal.py
--rw-r--r--   0 larsoner   (501) staff       (20)     4276 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-source-space/30_cluster_ftest_spatiotemporal.py
--rw-r--r--   0 larsoner   (501) staff       (20)    11262 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/stats-source-space/60_cluster_rmANOVA_spatiotemporal.py
--rw-r--r--   0 larsoner   (501) staff       (20)      162 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/stats-source-space/README.txt
-drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-05 16:28:42.251676 mne-1.4.1/tutorials/time-freq/
--rw-r--r--   0 larsoner   (501) staff       (20)     8044 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/time-freq/10_spectrum_class.py
--rw-r--r--   0 larsoner   (501) staff       (20)     7801 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/time-freq/20_sensors_time_frequency.py
--rw-r--r--   0 larsoner   (501) staff       (20)    26579 2023-06-05 14:01:41.000000 mne-1.4.1/tutorials/time-freq/50_ssvep.py
--rw-r--r--   0 larsoner   (501) staff       (20)      128 2022-11-28 17:38:21.000000 mne-1.4.1/tutorials/time-freq/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.701333 mne-1.4.2/
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.494158 mne-1.4.2/.circleci/
+-rw-r--r--   0 larsoner   (501) staff       (20)    18220 2023-06-06 14:38:39.000000 mne-1.4.2/.circleci/config.yml
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.494879 mne-1.4.2/.github/
+-rw-r--r--   0 larsoner   (501) staff       (20)      935 2022-11-28 17:38:20.000000 mne-1.4.2/.github/CODEOWNERS
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.495570 mne-1.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1933 2022-11-28 17:38:20.000000 mne-1.4.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)      258 2022-11-28 17:38:20.000000 mne-1.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)      900 2022-11-28 17:38:20.000000 mne-1.4.2/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)     1633 2022-11-28 17:38:20.000000 mne-1.4.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)     1004 2023-06-05 14:01:41.000000 mne-1.4.2/.github/config.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)      118 2022-11-28 17:38:20.000000 mne-1.4.2/.github/dependabot.yml
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.496019 mne-1.4.2/.github/workflows/
+-rw-r--r--   0 larsoner   (501) staff       (20)      575 2023-06-05 14:01:41.000000 mne-1.4.2/.github/workflows/circle_artifacts.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)     2742 2022-11-28 17:38:20.000000 mne-1.4.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)     3593 2023-06-05 14:01:41.000000 mne-1.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 larsoner   (501) staff       (20)     1057 2023-06-05 14:01:41.000000 mne-1.4.2/.gitignore
+-rw-r--r--   0 larsoner   (501) staff       (20)     1527 2022-11-28 17:38:20.000000 mne-1.4.2/LICENSE.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2534 2023-06-05 14:01:41.000000 mne-1.4.2/MANIFEST.in
+-rw-r--r--   0 larsoner   (501) staff       (20)     6944 2023-06-06 14:44:59.701174 mne-1.4.2/PKG-INFO
+-rw-r--r--   0 larsoner   (501) staff       (20)     5607 2023-06-05 14:01:41.000000 mne-1.4.2/README.rst
+-rw-r--r--   0 larsoner   (501) staff       (20)     1343 2023-06-05 14:01:41.000000 mne-1.4.2/SECURITY.md
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.496204 mne-1.4.2/examples/
+-rw-r--r--   0 larsoner   (501) staff       (20)      794 2022-11-28 17:38:20.000000 mne-1.4.2/examples/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.496475 mne-1.4.2/examples/connectivity/
+-rw-r--r--   0 larsoner   (501) staff       (20)      326 2022-11-28 17:38:20.000000 mne-1.4.2/examples/connectivity/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.497688 mne-1.4.2/examples/datasets/
+-rw-r--r--   0 larsoner   (501) staff       (20)      102 2022-05-20 17:14:56.000000 mne-1.4.2/examples/datasets/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2095 2023-06-05 14:01:41.000000 mne-1.4.2/examples/datasets/brainstorm_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      737 2023-06-05 14:01:41.000000 mne-1.4.2/examples/datasets/hf_sef_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10907 2023-06-05 14:01:41.000000 mne-1.4.2/examples/datasets/limo_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4484 2023-06-05 14:01:41.000000 mne-1.4.2/examples/datasets/opm_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4287 2023-06-05 14:01:41.000000 mne-1.4.2/examples/datasets/spm_faces_dataset_sgskip.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.499476 mne-1.4.2/examples/decoding/
+-rw-r--r--   0 larsoner   (501) staff       (20)      157 2022-05-20 17:14:56.000000 mne-1.4.2/examples/decoding/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     4745 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_csp_eeg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5964 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_csp_timefreq.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6879 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_rsa_sgskip.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4241 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_spatio_temporal_source.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2969 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_spoc_CMC.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3496 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_time_generalization_conditions.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2462 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_unsupervised_spatial_filter.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3912 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/decoding_xdawn_eeg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4727 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/ems_filtering.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4035 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/linear_model_patterns.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10675 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/receptive_field_mtrf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4816 2023-06-05 14:01:41.000000 mne-1.4.2/examples/decoding/ssd_spatial_filters.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.500045 mne-1.4.2/examples/forward/
+-rw-r--r--   0 larsoner   (501) staff       (20)      143 2022-05-20 17:14:56.000000 mne-1.4.2/examples/forward/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     3718 2023-06-05 14:01:41.000000 mne-1.4.2/examples/forward/forward_sensitivity_maps.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2135 2023-06-05 14:01:41.000000 mne-1.4.2/examples/forward/left_cerebellum_volume_source.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2611 2023-06-05 14:01:41.000000 mne-1.4.2/examples/forward/source_space_morphing.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.504764 mne-1.4.2/examples/inverse/
+-rw-r--r--   0 larsoner   (501) staff       (20)      168 2022-05-20 17:14:56.000000 mne-1.4.2/examples/inverse/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     4119 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/compute_mne_inverse_epochs_in_label.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1641 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/compute_mne_inverse_raw_in_label.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1680 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/compute_mne_inverse_volume.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6385 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/custom_inverse_solver.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4304 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/dics_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3461 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/dics_source_power.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5649 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/evoked_ers_source_power.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3193 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/gamma_map_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2073 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/label_activation_from_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3785 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/label_from_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3449 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/label_source_activations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4774 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/mixed_norm_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5692 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/mixed_source_space_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4872 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/mne_cov_power.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5790 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/morph_surface_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6119 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/morph_volume_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7462 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/multi_dipole_model.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3411 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/multidict_reweighted_tfmxne.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7183 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/psf_ctf_label_leakage.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3190 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/psf_ctf_vertices.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4888 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/psf_ctf_vertices_lcmv.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3005 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/psf_volume.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1678 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/rap_music.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1467 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/read_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      760 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/read_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4791 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/resolution_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5248 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/resolution_metrics_eegmeg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      780 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/snr_estimate.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2489 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/source_space_snr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5042 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/time_frequency_mixed_norm_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1704 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/trap_music.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3671 2023-06-05 14:01:41.000000 mne-1.4.2/examples/inverse/vector_mne_solution.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.505582 mne-1.4.2/examples/io/
+-rw-r--r--   0 larsoner   (501) staff       (20)      262 2022-11-28 17:38:20.000000 mne-1.4.2/examples/io/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2073 2023-06-05 14:01:41.000000 mne-1.4.2/examples/io/elekta_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1356 2023-06-05 14:01:41.000000 mne-1.4.2/examples/io/read_neo_format.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      654 2023-06-05 14:01:41.000000 mne-1.4.2/examples/io/read_noise_covariance_matrix.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1193 2023-06-05 14:01:41.000000 mne-1.4.2/examples/io/read_xdf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.508841 mne-1.4.2/examples/preprocessing/
+-rw-r--r--   0 larsoner   (501) staff       (20)      697 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2309 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/contralateral_referencing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3808 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/css.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3162 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/define_target_events.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17460 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/eeg_bridging.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2934 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/eeg_csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1405 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/eog_artifact_histogram.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2407 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/eog_regression.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4818 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/find_ref_artifacts.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3096 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/fnirs_artifact_removal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1497 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/ica_comparison.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1453 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/interpolate_bad_channels.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2908 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/movement_compensation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3516 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/movement_detection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3021 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/muscle_detection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4382 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/muscle_ica.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2936 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/otp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1304 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/shift_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1608 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/virtual_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2593 2023-06-05 14:01:41.000000 mne-1.4.2/examples/preprocessing/xdawn_denoising.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.509771 mne-1.4.2/examples/simulation/
+-rw-r--r--   0 larsoner   (501) staff       (20)       69 2022-05-20 17:14:56.000000 mne-1.4.2/examples/simulation/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     8699 2023-06-05 14:01:41.000000 mne-1.4.2/examples/simulation/plot_stc_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2450 2023-06-05 14:01:41.000000 mne-1.4.2/examples/simulation/simulate_evoked_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2820 2023-06-05 14:01:41.000000 mne-1.4.2/examples/simulation/simulate_raw_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8569 2023-06-05 14:01:41.000000 mne-1.4.2/examples/simulation/simulated_raw_data_using_subject_anatomy.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3293 2023-06-05 14:01:41.000000 mne-1.4.2/examples/simulation/source_simulator.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.510651 mne-1.4.2/examples/stats/
+-rw-r--r--   0 larsoner   (501) staff       (20)      110 2022-05-20 17:14:56.000000 mne-1.4.2/examples/stats/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2640 2023-06-05 14:01:41.000000 mne-1.4.2/examples/stats/cluster_stats_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2501 2023-06-05 14:01:41.000000 mne-1.4.2/examples/stats/fdr_stats_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2404 2023-06-05 14:01:41.000000 mne-1.4.2/examples/stats/linear_regression_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2268 2023-06-05 14:01:41.000000 mne-1.4.2/examples/stats/sensor_permutation_test.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3759 2023-06-05 14:01:41.000000 mne-1.4.2/examples/stats/sensor_regression.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.512624 mne-1.4.2/examples/time_frequency/
+-rw-r--r--   0 larsoner   (501) staff       (20)      129 2022-05-20 17:14:56.000000 mne-1.4.2/examples/time_frequency/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     3857 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/compute_csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3165 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/compute_source_psd_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3682 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/source_label_time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1814 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/source_power_spectrum.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7980 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/source_power_spectrum_opm.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2179 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/source_space_time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1791 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/temporal_whitening.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7949 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/time_frequency_erds.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4999 2023-06-05 14:01:41.000000 mne-1.4.2/examples/time_frequency/time_frequency_global_field_power.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9775 2023-06-06 14:38:39.000000 mne-1.4.2/examples/time_frequency/time_frequency_simulated.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.515627 mne-1.4.2/examples/visualization/
+-rw-r--r--   0 larsoner   (501) staff       (20)     4787 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/3d_to_2d.py
+-rw-r--r--   0 larsoner   (501) staff       (20)       69 2022-05-20 17:14:56.000000 mne-1.4.2/examples/visualization/README.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     4312 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/brain.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2476 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/channel_epochs_image.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      908 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/eeg_on_scalp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2673 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/evoked_arrowmap.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6656 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/evoked_topomap.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2677 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/evoked_whitening.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1970 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/meg_sensors.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1319 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/mne_helmet.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2100 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/montage_sgskip.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2044 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/parcellation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10240 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/publication_figure.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3156 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/roi_erpimage_by_rt.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      772 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/sensor_noise_level.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1224 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/ssp_projs_sensitivity_map.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1692 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/topo_compare_conditions.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1909 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/topo_customized.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1391 2023-06-05 14:01:41.000000 mne-1.4.2/examples/visualization/xhemi.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.526793 mne-1.4.2/mne/
+-rw-r--r--   0 larsoner   (501) staff       (20)     5666 2023-06-06 14:38:39.000000 mne-1.4.2/mne/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      144 2023-06-05 14:01:41.000000 mne-1.4.2/mne/__main__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    27654 2023-06-05 14:01:41.000000 mne-1.4.2/mne/_freesurfer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19447 2023-06-05 14:01:41.000000 mne-1.4.2/mne/_ola.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      176 2023-06-06 14:44:58.000000 mne-1.4.2/mne/_version.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    63163 2023-06-05 14:01:41.000000 mne-1.4.2/mne/annotations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6831 2023-06-06 14:38:39.000000 mne-1.4.2/mne/baseline.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.529203 mne-1.4.2/mne/beamformer/
+-rw-r--r--   0 larsoner   (501) staff       (20)      474 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20475 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/_compute_beamformer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21949 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/_dics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15860 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/_lcmv.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10057 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/_rap_music.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2833 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/resolution_matrix.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.530132 mne-1.4.2/mne/beamformer/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/beamformer/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    35200 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/tests/test_dics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4171 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/tests/test_external.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    42658 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/tests/test_lcmv.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8040 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/tests/test_rap_music.py
+-rwxr-xr-x   0 larsoner   (501) staff       (20)     3313 2023-06-05 14:01:41.000000 mne-1.4.2/mne/beamformer/tests/test_resolution_matrix.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    86946 2023-06-05 14:01:41.000000 mne-1.4.2/mne/bem.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.532215 mne-1.4.2/mne/channels/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1854 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3120 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/_dig_montage_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14208 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/_standard_montage_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    84931 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/channels.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.481212 mne-1.4.2/mne/channels/data/
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.535681 mne-1.4.2/mne/channels/data/layouts/
+-rw-r--r--   0 larsoner   (501) staff       (20)    14061 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/CTF-275.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     7154 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/CTF151.lay
+-rw-r--r--   0 larsoner   (501) staff       (20)    12807 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/CTF275.lay
+-rw-r--r--   0 larsoner   (501) staff       (20)    15343 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/EEG1005.lay
+-rw-r--r--   0 larsoner   (501) staff       (20)    15526 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/EGI256.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     5823 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/GeodesicHeadWeb-130.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)    12573 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/GeodesicHeadWeb-280.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     6036 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/layouts/KIT-125.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     7562 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/KIT-157.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)    10895 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/layouts/KIT-160.lay
+-rw-r--r--   0 larsoner   (501) staff       (20)    10020 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/KIT-AD.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     7572 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/KIT-AS-2008.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     7572 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/KIT-UMD-3.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     4406 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/layouts/Neuromag_122.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)    16054 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/Vectorview-all.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)    10704 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/Vectorview-grad.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     5256 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/Vectorview-grad_norm.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     5358 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/Vectorview-mag.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)     2770 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/layouts/biosemi.lay
+-rw-r--r--   0 larsoner   (501) staff       (20)    11940 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/layouts/magnesWH3600.lout
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.539992 mne-1.4.2/mne/channels/data/montages/
+-rw-r--r--   0 larsoner   (501) staff       (20)    24999 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/EGI_256.csd
+-rw-r--r--   0 larsoner   (501) staff       (20)     5297 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-128.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     5316 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-129.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     7796 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-256.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     7823 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-257.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     1382 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-32.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     2877 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-64_1.0.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)     2919 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-65_1.0.sfp
+-rw-r--r--   0 larsoner   (501) staff       (20)      544 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/montages/artinis-brite23.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)      376 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/montages/artinis-octamon.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     1555 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi128.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      248 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi16.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     1910 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi160.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     3354 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi256.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      453 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi32.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      710 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/biosemi64.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2358 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/montages/brainproducts-RNP-BA-128.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      947 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/easycap-M1.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      800 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/easycap-M10.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2110 2023-04-21 22:27:15.000000 mne-1.4.2/mne/channels/data/montages/mgh60.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     2428 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/montages/mgh70.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)    10478 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_1005.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     2896 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_1020.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     2009 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_alphabetic.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     3066 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_postfixed.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     2305 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_prefixed.elc
+-rw-r--r--   0 larsoner   (501) staff       (20)     3093 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/montages/standard_primed.elc
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.545563 mne-1.4.2/mne/channels/data/neighbors/
+-rw-r--r--   0 larsoner   (501) staff       (20)     4939 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-157_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     6636 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-208_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4990 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-NYU-2019_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4750 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-1_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4832 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-2_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4794 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-3_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4840 2022-11-28 17:38:12.000000 mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-4_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)      487 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/data/neighbors/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      511 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/biosemi16_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)      942 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/biosemi32_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1812 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/biosemi64_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     3920 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/bti148_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     6577 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/bti248_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     8337 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/bti248grad_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4380 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/ctf151_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     7831 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/ctf275_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2397 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/ctf64_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     3870 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycap128ch-avg_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1127 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycap32ch-avg_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1861 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycap64ch-avg_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1792 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycapM11_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     3529 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycapM14_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     3906 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycapM15_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2149 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/easycapM1_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     6286 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/ecog256_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4221 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/ecog256bipolar_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2422 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/eeg1010_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)    11892 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/elec1005_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2390 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/elec1010_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)      655 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/elec1020_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4045 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/itab153_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)      743 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/itab28_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1135 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/language29ch-avg_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     1660 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/mpi_59_channels_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2074 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/neuromag122cmb_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     3685 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/neuromag306cmb_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     2753 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/neuromag306mag_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     5580 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/neuromag306planar_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     4729 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/yokogawa160_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)    15521 2022-11-28 17:38:21.000000 mne-1.4.2/mne/channels/data/neighbors/yokogawa440_neighb.mat
+-rw-r--r--   0 larsoner   (501) staff       (20)     8789 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/interpolation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    39984 2023-06-06 14:38:39.000000 mne-1.4.2/mne/channels/layout.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    59199 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/montage.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.547045 mne-1.4.2/mne/channels/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/channels/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26410 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/tests/test_channels.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12511 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/tests/test_interpolation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15138 2023-06-06 14:38:39.000000 mne-1.4.2/mne/channels/tests/test_layout.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    72846 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/tests/test_montage.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10249 2023-06-05 14:01:41.000000 mne-1.4.2/mne/channels/tests/test_standard_montage.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    55540 2023-06-05 14:01:41.000000 mne-1.4.2/mne/chpi.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.550752 mne-1.4.2/mne/commands/
+-rw-r--r--   0 larsoner   (501) staff       (20)       51 2022-05-20 17:14:56.000000 mne-1.4.2/mne/commands/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3283 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_anonymize.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5425 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_browse_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3297 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_bti2fiff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5876 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_clean_eog_ecg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      538 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_compare_fiff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8344 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_compute_proj_ecg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8354 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_compute_proj_eog.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3904 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5131 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_flash_bem.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3294 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_freeview_bem_surfaces.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2700 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_kit2fiff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2503 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_make_scalp_surfaces.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6362 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_maxfilter.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1654 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_prepare_bem_model.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6116 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_report.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4224 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_setup_forward_model.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4982 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_setup_source_space.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      783 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_show_fiff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      695 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_show_info.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1212 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_surf2bem.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1177 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_sys_info.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3196 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_watershed_bem.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      473 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/mne_what.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.551011 mne-1.4.2/mne/commands/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/commands/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16859 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/tests/test_commands.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3102 2023-06-05 14:01:41.000000 mne-1.4.2/mne/commands/utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    35658 2023-06-06 14:38:39.000000 mne-1.4.2/mne/conftest.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    78521 2023-06-05 14:01:41.000000 mne-1.4.2/mne/coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    80732 2023-06-05 14:01:41.000000 mne-1.4.2/mne/cov.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12277 2023-06-05 14:01:41.000000 mne-1.4.2/mne/cuda.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.557704 mne-1.4.2/mne/data/
+-rw-r--r--   0 larsoner   (501) staff       (20)    84835 2022-11-28 17:38:21.000000 mne-1.4.2/mne/data/FreeSurferColorLUT.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)       23 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    51080 2022-11-28 17:38:21.000000 mne-1.4.2/mne/data/coil_def.dat
+-rw-r--r--   0 larsoner   (501) staff       (20)     5064 2022-11-28 17:38:12.000000 mne-1.4.2/mne/data/coil_def_Elekta.dat
+-rw-r--r--   0 larsoner   (501) staff       (20)   293567 2022-11-28 17:38:21.000000 mne-1.4.2/mne/data/eegbci_checksums.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     3419 2022-11-28 17:38:12.000000 mne-1.4.2/mne/data/extinction_coef.mat
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.560623 mne-1.4.2/mne/data/fsaverage/
+-rw-r--r--   0 larsoner   (501) staff       (20)      260 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/fsaverage/fsaverage-fiducials.fif
+-rw-r--r--   0 larsoner   (501) staff       (20)    97892 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/fsaverage/fsaverage-head.fif
+-rw-r--r--   0 larsoner   (501) staff       (20)   491944 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/fsaverage/fsaverage-inner_skull-bem.fif
+-rw-r--r--   0 larsoner   (501) staff       (20)      212 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/fsaverage/fsaverage-trans.fif
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.561934 mne-1.4.2/mne/data/helmets/
+-rw-r--r--   0 larsoner   (501) staff       (20)     4706 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/122m.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)     9462 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/306m.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)     9443 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/306m_rt.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)    59505 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/BabySQUID.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)    11157 2022-11-28 17:38:12.000000 mne-1.4.2/mne/data/helmets/CTF_275.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)     9477 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/KIT.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)     9470 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/Magnes_2500wh.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)     9475 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/helmets/Magnes_3600wh.fif.gz
+-rw-r--r--   0 larsoner   (501) staff       (20)  3732551 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/icos.fif.gz
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.562241 mne-1.4.2/mne/data/image/
+-rw-r--r--   0 larsoner   (501) staff       (20)    11190 2022-11-28 17:38:21.000000 mne-1.4.2/mne/data/image/custom_layout.lout
+-rw-r--r--   0 larsoner   (501) staff       (20)    12051 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/image/mni_brain.gif
+-rw-r--r--   0 larsoner   (501) staff       (20)     4320 2022-05-20 17:14:56.000000 mne-1.4.2/mne/data/mne_analyze.sel
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.563153 mne-1.4.2/mne/datasets/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1620 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/__init__.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.563752 mne-1.4.2/mne/datasets/_fake/
+-rw-r--r--   0 larsoner   (501) staff       (20)       75 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/_fake/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      844 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/_fake/_fake.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11863 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/_fetch.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.564325 mne-1.4.2/mne/datasets/_fsaverage/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/_fsaverage/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4563 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/_fsaverage/base.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      320 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/_fsaverage/bem.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     5795 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/_fsaverage/root.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.566530 mne-1.4.2/mne/datasets/_infant/
+-rw-r--r--   0 larsoner   (501) staff       (20)     2499 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS1-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2475 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS10-5Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS12-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS15-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2689 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS18-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2499 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS2-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2493 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS2-0Weeks3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2677 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS2-0Years3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS3-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS4-5Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS6-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS7-5Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     2683 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_infant/ANTS9-0Months3T.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     3866 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/_infant/base.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.566934 mne-1.4.2/mne/datasets/_phantom/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_phantom/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1834 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/_phantom/base.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      113 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/_phantom/phantom_otaniemi.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.567835 mne-1.4.2/mne/datasets/brainstorm/
+-rw-r--r--   0 larsoner   (501) staff       (20)      114 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1789 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/bst_auditory.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1263 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/bst_phantom_ctf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1281 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/bst_phantom_elekta.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2298 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/bst_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1335 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/brainstorm/bst_resting.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13748 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/config.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.568123 mne-1.4.2/mne/datasets/eegbci/
+-rw-r--r--   0 larsoner   (501) staff       (20)       97 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/eegbci/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7973 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/eegbci/eegbci.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.568269 mne-1.4.2/mne/datasets/eegbci/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)      397 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/eegbci/tests/test_eegbci.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.568579 mne-1.4.2/mne/datasets/epilepsy_ecog/
+-rw-r--r--   0 larsoner   (501) staff       (20)       77 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/epilepsy_ecog/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      820 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/epilepsy_ecog/_data.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.568922 mne-1.4.2/mne/datasets/erp_core/
+-rw-r--r--   0 larsoner   (501) staff       (20)       74 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/erp_core/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      682 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/erp_core/erp_core.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.569397 mne-1.4.2/mne/datasets/eyelink/
+-rw-r--r--   0 larsoner   (501) staff       (20)       73 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/eyelink/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      748 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/eyelink/eyelink.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.569840 mne-1.4.2/mne/datasets/fieldtrip_cmc/
+-rw-r--r--   0 larsoner   (501) staff       (20)      109 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/fieldtrip_cmc/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      852 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/fieldtrip_cmc/fieldtrip_cmc.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.570217 mne-1.4.2/mne/datasets/fnirs_motor/
+-rw-r--r--   0 larsoner   (501) staff       (20)       76 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/fnirs_motor/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      769 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/fnirs_motor/fnirs_motor.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.570658 mne-1.4.2/mne/datasets/hf_sef/
+-rw-r--r--   0 larsoner   (501) staff       (20)       53 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/hf_sef/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2867 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/hf_sef/hf_sef.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.571047 mne-1.4.2/mne/datasets/kiloword/
+-rw-r--r--   0 larsoner   (501) staff       (20)       86 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/kiloword/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1989 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/kiloword/kiloword.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.571386 mne-1.4.2/mne/datasets/limo/
+-rw-r--r--   0 larsoner   (501) staff       (20)       60 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/limo/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13058 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/limo/limo.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.571723 mne-1.4.2/mne/datasets/misc/
+-rw-r--r--   0 larsoner   (501) staff       (20)       68 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/misc/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      851 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/misc/_misc.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.572057 mne-1.4.2/mne/datasets/mtrf/
+-rw-r--r--   0 larsoner   (501) staff       (20)       62 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/mtrf/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      765 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/mtrf/mtrf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.572368 mne-1.4.2/mne/datasets/multimodal/
+-rw-r--r--   0 larsoner   (501) staff       (20)       74 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/multimodal/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      879 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/multimodal/multimodal.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.572733 mne-1.4.2/mne/datasets/opm/
+-rw-r--r--   0 larsoner   (501) staff       (20)       60 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/opm/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      839 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/opm/opm.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.573015 mne-1.4.2/mne/datasets/phantom_4dbti/
+-rw-r--r--   0 larsoner   (501) staff       (20)       77 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/phantom_4dbti/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      792 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/phantom_4dbti/phantom_4dbti.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.573273 mne-1.4.2/mne/datasets/refmeg_noise/
+-rw-r--r--   0 larsoner   (501) staff       (20)       86 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/refmeg_noise/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      770 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/refmeg_noise/refmeg_noise.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.573532 mne-1.4.2/mne/datasets/sample/
+-rw-r--r--   0 larsoner   (501) staff       (20)       70 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/sample/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      859 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/sample/sample.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.574808 mne-1.4.2/mne/datasets/sleep_physionet/
+-rw-r--r--   0 larsoner   (501) staff       (20)    24428 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/sleep_physionet/SHA1SUMS
+-rw-r--r--   0 larsoner   (501) staff       (20)       37 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/sleep_physionet/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8092 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/sleep_physionet/_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5127 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/sleep_physionet/age.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    27887 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/sleep_physionet/age_records.csv
+-rw-r--r--   0 larsoner   (501) staff       (20)     3772 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/sleep_physionet/temazepam.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6990 2022-11-28 17:38:12.000000 mne-1.4.2/mne/datasets/sleep_physionet/temazepam_records.csv
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.574940 mne-1.4.2/mne/datasets/sleep_physionet/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     7287 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/sleep_physionet/tests/test_physionet.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.575316 mne-1.4.2/mne/datasets/somato/
+-rw-r--r--   0 larsoner   (501) staff       (20)       73 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/somato/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      859 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/somato/somato.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.575672 mne-1.4.2/mne/datasets/spm_face/
+-rw-r--r--   0 larsoner   (501) staff       (20)      103 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/spm_face/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1203 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/spm_face/spm_data.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.575952 mne-1.4.2/mne/datasets/ssvep/
+-rw-r--r--   0 larsoner   (501) staff       (20)       64 2022-11-28 17:38:21.000000 mne-1.4.2/mne/datasets/ssvep/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      732 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/ssvep/ssvep.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.576214 mne-1.4.2/mne/datasets/testing/
+-rw-r--r--   0 larsoner   (501) staff       (20)      150 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/testing/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2119 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/testing/_testing.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.576417 mne-1.4.2/mne/datasets/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12452 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/tests/test_datasets.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.576772 mne-1.4.2/mne/datasets/ucl_opm_auditory/
+-rw-r--r--   0 larsoner   (501) staff       (20)       81 2023-04-24 01:19:07.000000 mne-1.4.2/mne/datasets/ucl_opm_auditory/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      800 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/ucl_opm_auditory/ucl_opm_auditory.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    28071 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/utils.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.577038 mne-1.4.2/mne/datasets/visual_92_categories/
+-rw-r--r--   0 larsoner   (501) staff       (20)       98 2022-05-20 17:14:56.000000 mne-1.4.2/mne/datasets/visual_92_categories/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2182 2023-06-05 14:01:41.000000 mne-1.4.2/mne/datasets/visual_92_categories/visual_92_categories.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.579295 mne-1.4.2/mne/decoding/
+-rw-r--r--   0 larsoner   (501) staff       (20)      624 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19127 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/base.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    29368 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/csp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7623 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/ems.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2863 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/mixin.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19219 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/receptive_field.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26793 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/search_light.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14734 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/ssd.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.580755 mne-1.4.2/mne/decoding/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/decoding/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15649 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_base.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13441 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_csp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3134 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_ems.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22450 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_receptive_field.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10791 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_search_light.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13993 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_ssd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1351 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9655 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/tests/test_transformer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13577 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/time_delaying_ridge.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5130 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    29890 2023-06-05 14:01:41.000000 mne-1.4.2/mne/decoding/transformer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9083 2023-06-05 14:01:41.000000 mne-1.4.2/mne/defaults.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    59776 2023-06-05 14:01:41.000000 mne-1.4.2/mne/dipole.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   156962 2023-06-05 14:01:41.000000 mne-1.4.2/mne/epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    58244 2023-06-06 14:38:39.000000 mne-1.4.2/mne/event.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    63030 2023-06-05 14:01:41.000000 mne-1.4.2/mne/evoked.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.581888 mne-1.4.2/mne/export/
+-rw-r--r--   0 larsoner   (501) staff       (20)      103 2022-11-28 17:38:21.000000 mne-1.4.2/mne/export/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      472 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/_brainvision.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12063 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/_edf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2510 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/_eeglab.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5620 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/_egimff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6010 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/_export.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.582037 mne-1.4.2/mne/export/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)    19429 2023-06-05 14:01:41.000000 mne-1.4.2/mne/export/tests/test_export.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    95360 2023-06-05 14:01:41.000000 mne-1.4.2/mne/filter.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    31217 2023-06-05 14:01:41.000000 mne-1.4.2/mne/fixes.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.583382 mne-1.4.2/mne/forward/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1123 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    34441 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/_compute_forward.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18408 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/_field_interpolation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19463 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/_lead_dots.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    31718 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/_make_forward.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    77927 2023-06-06 14:38:39.000000 mne-1.4.2/mne/forward/forward.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.584382 mne-1.4.2/mne/forward/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/forward/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11446 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/tests/test_field_interpolation.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18572 2023-06-06 14:38:39.000000 mne-1.4.2/mne/forward/tests/test_forward.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    30292 2023-06-05 14:01:41.000000 mne-1.4.2/mne/forward/tests/test_make_forward.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.585101 mne-1.4.2/mne/gui/
+-rw-r--r--   0 larsoner   (501) staff       (20)    12864 2023-06-06 14:38:39.000000 mne-1.4.2/mne/gui/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    23226 2023-06-06 14:38:39.000000 mne-1.4.2/mne/gui/_core.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    76082 2023-06-05 14:01:41.000000 mne-1.4.2/mne/gui/_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    33695 2023-06-06 14:38:39.000000 mne-1.4.2/mne/gui/_ieeg_locate.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.585865 mne-1.4.2/mne/gui/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/gui/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2273 2023-06-06 14:38:39.000000 mne-1.4.2/mne/gui/tests/test_core.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12760 2023-06-05 14:01:41.000000 mne-1.4.2/mne/gui/tests/test_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11178 2023-06-05 14:01:41.000000 mne-1.4.2/mne/gui/tests/test_gui_api.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8479 2023-06-06 14:38:39.000000 mne-1.4.2/mne/gui/tests/test_ieeg_locate.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.586649 mne-1.4.2/mne/html/
+-rw-r--r--   0 larsoner   (501) staff       (20)   146814 2022-05-20 17:14:56.000000 mne-1.4.2/mne/html/d3.v3.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)    36228 2022-05-20 17:14:56.000000 mne-1.4.2/mne/html/mpld3.v0.2.min.js
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.587110 mne-1.4.2/mne/html_templates/
+-rw-r--r--   0 larsoner   (501) staff       (20)       95 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      509 2023-06-05 14:01:41.000000 mne-1.4.2/mne/html_templates/_templates.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.590024 mne-1.4.2/mne/html_templates/report/
+-rw-r--r--   0 larsoner   (501) staff       (20)      217 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/bem.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      172 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/code.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      287 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/footer.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      132 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/forward.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)     1864 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/header.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      892 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/html.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      535 2023-06-05 14:01:41.000000 mne-1.4.2/mne/html_templates/report/image.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      128 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/inverse.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      993 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/section.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)     2812 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/slider.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      610 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/report/toc.html.jinja
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.591203 mne-1.4.2/mne/html_templates/repr/
+-rw-r--r--   0 larsoner   (501) staff       (20)      599 2023-06-05 14:01:41.000000 mne-1.4.2/mne/html_templates/repr/epochs.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      689 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/evoked.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      449 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/forward.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      811 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/ica.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)     1836 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/info.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      354 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/inverse_operator.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)      256 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/raw.html.jinja
+-rw-r--r--   0 larsoner   (501) staff       (20)     1329 2022-11-28 17:38:21.000000 mne-1.4.2/mne/html_templates/repr/spectrum.html.jinja
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.592877 mne-1.4.2/mne/icons/
+-rw-r--r--   0 larsoner   (501) staff       (20)      290 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/README.rst
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.593024 mne-1.4.2/mne/icons/dark/
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.594709 mne-1.4.2/mne/icons/dark/actions/
+-rw-r--r--   0 larsoner   (501) staff       (20)      252 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/clear.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      276 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/folder.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      402 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/help.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      442 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/movie.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      452 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/pause.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      405 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/play.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      372 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/reset.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      377 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/restore.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      685 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/scale.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      396 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/screenshot.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      901 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/visibility_off.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      493 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/actions/visibility_on.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      116 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/dark/index.theme
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.594846 mne-1.4.2/mne/icons/light/
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.596586 mne-1.4.2/mne/icons/light/actions/
+-rw-r--r--   0 larsoner   (501) staff       (20)      252 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/clear.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      276 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/folder.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      402 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/help.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      442 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/movie.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      452 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/pause.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      405 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/play.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      372 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/reset.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      377 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/restore.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      685 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/scale.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      396 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/screenshot.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      901 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/visibility_off.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      493 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/actions/visibility_on.svg
+-rw-r--r--   0 larsoner   (501) staff       (20)      117 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/light/index.theme
+-rw-r--r--   0 larsoner   (501) staff       (20)    44028 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/mne_bigsur_icon.png
+-rw-r--r--   0 larsoner   (501) staff       (20)    10369 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/mne_default_icon.png
+-rw-r--r--   0 larsoner   (501) staff       (20)    44818 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/mne_icon-cropped.png
+-rw-r--r--   0 larsoner   (501) staff       (20)    31258 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/mne_icon.png
+-rw-r--r--   0 larsoner   (501) staff       (20)    22283 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/mne_splash.png
+-rw-r--r--   0 larsoner   (501) staff       (20)      304 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/toolbar_move_horizontal@2x.png
+-rw-r--r--   0 larsoner   (501) staff       (20)      208 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/toolbar_move_vertical@2x.png
+-rw-r--r--   0 larsoner   (501) staff       (20)      151 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/toolbar_separator_horizontal.png
+-rw-r--r--   0 larsoner   (501) staff       (20)      288 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/toolbar_separator_horizontal@2x.png
+-rw-r--r--   0 larsoner   (501) staff       (20)      192 2022-11-28 17:38:21.000000 mne-1.4.2/mne/icons/toolbar_separator_vertical@2x.png
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.597451 mne-1.4.2/mne/inverse_sparse/
+-rw-r--r--   0 larsoner   (501) staff       (20)      239 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10212 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/_gamma_map.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3564 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/mxne_debiasing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    35158 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/mxne_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    54504 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/mxne_optim.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.598376 mne-1.4.2/mne/inverse_sparse/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/inverse_sparse/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6754 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/tests/test_gamma_map.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      807 2022-11-28 17:38:21.000000 mne-1.4.2/mne/inverse_sparse/tests/test_mxne_debiasing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19290 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/tests/test_mxne_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14735 2023-06-05 14:01:41.000000 mne-1.4.2/mne/inverse_sparse/tests/test_mxne_optim.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.604115 mne-1.4.2/mne/io/
+-rw-r--r--   0 larsoner   (501) staff       (20)     2231 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20833 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/_digitization.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4589 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/_read_raw.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.604516 mne-1.4.2/mne/io/array/
+-rw-r--r--   0 larsoner   (501) staff       (20)      120 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/array/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3234 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/array/array.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.604850 mne-1.4.2/mne/io/array/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/array/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6725 2023-06-06 14:38:39.000000 mne-1.4.2/mne/io/array/tests/test_array.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.605631 mne-1.4.2/mne/io/artemis123/
+-rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/artemis123/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19620 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/artemis123/artemis123.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.606171 mne-1.4.2/mne/io/artemis123/resources/
+-rw-r--r--   0 larsoner   (501) staff       (20)     9272 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/artemis123/resources/Artemis123_ChannelMap.csv
+-rw-r--r--   0 larsoner   (501) staff       (20)    25854 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/artemis123/resources/Artemis123_mneLoc.csv
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.606698 mne-1.4.2/mne/io/artemis123/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/artemis123/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4407 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/artemis123/tests/test_artemis123.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4365 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/artemis123/utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   105890 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/base.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.607088 mne-1.4.2/mne/io/besa/
+-rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/besa/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8977 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/besa/besa.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.607349 mne-1.4.2/mne/io/besa/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     2890 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/besa/tests/test_besa.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.607858 mne-1.4.2/mne/io/boxy/
+-rw-r--r--   0 larsoner   (501) staff       (20)      166 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/boxy/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11481 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/boxy/boxy.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.608109 mne-1.4.2/mne/io/boxy/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/boxy/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7599 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/boxy/tests/test_boxy.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.608469 mne-1.4.2/mne/io/brainvision/
+-rw-r--r--   0 larsoner   (501) staff       (20)      226 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/brainvision/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    41837 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/brainvision/brainvision.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.608884 mne-1.4.2/mne/io/brainvision/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        1 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/brainvision/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    31664 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/brainvision/tests/test_brainvision.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.610286 mne-1.4.2/mne/io/bti/
+-rw-r--r--   0 larsoner   (501) staff       (20)      127 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/bti/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    52902 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/bti/bti.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2323 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/bti/constants.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2878 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/bti/read.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.610550 mne-1.4.2/mne/io/bti/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/bti/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17651 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/bti/tests/test_bti.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.611117 mne-1.4.2/mne/io/cnt/
+-rw-r--r--   0 larsoner   (501) staff       (20)       54 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/cnt/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4767 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/cnt/_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22378 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/cnt/cnt.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.611379 mne-1.4.2/mne/io/cnt/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/cnt/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1973 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/cnt/tests/test_cnt.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5667 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/compensator.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    40164 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/constants.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.613068 mne-1.4.2/mne/io/ctf/
+-rw-r--r--   0 larsoner   (501) staff       (20)      154 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/ctf/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      726 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/constants.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11047 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/ctf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3781 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/eeg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2492 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/hc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20449 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/info.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2865 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/markers.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7078 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/res4.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.613291 mne-1.4.2/mne/io/ctf/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/ctf/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    24782 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/tests/test_ctf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4778 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf/trans.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5884 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/ctf_comp.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.613738 mne-1.4.2/mne/io/curry/
+-rw-r--r--   0 larsoner   (501) staff       (20)      144 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/curry/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21398 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/curry/curry.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.614019 mne-1.4.2/mne/io/curry/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.2/mne/io/curry/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18899 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/curry/tests/test_curry.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1217 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/diff.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.614375 mne-1.4.2/mne/io/edf/
+-rw-r--r--   0 larsoner   (501) staff       (20)      177 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/edf/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    71710 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/edf/edf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.615357 mne-1.4.2/mne/io/edf/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/edf/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    28995 2023-06-06 14:38:39.000000 mne-1.4.2/mne/io/edf/tests/test_edf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5920 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/edf/tests/test_gdf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.615823 mne-1.4.2/mne/io/eeglab/
+-rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:12.000000 mne-1.4.2/mne/io/eeglab/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2496 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eeglab/_eeglab.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    27991 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eeglab/eeglab.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.616103 mne-1.4.2/mne/io/eeglab/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/eeglab/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22820 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eeglab/tests/test_eeglab.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.616968 mne-1.4.2/mne/io/egi/
+-rw-r--r--   0 larsoner   (501) staff       (20)      164 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/egi/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11929 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/egi/egi.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    40256 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/egi/egimff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4726 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/egi/events.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6230 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/egi/general.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.617188 mne-1.4.2/mne/io/egi/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/egi/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19662 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/egi/tests/test_egi.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.617586 mne-1.4.2/mne/io/eximia/
+-rw-r--r--   0 larsoner   (501) staff       (20)      155 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/eximia/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3185 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eximia/eximia.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.617917 mne-1.4.2/mne/io/eximia/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/eximia/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1622 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eximia/tests/test_eximia.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.618323 mne-1.4.2/mne/io/eyelink/
+-rw-r--r--   0 larsoner   (501) staff       (20)      156 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eyelink/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    36953 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eyelink/eyelink.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.618605 mne-1.4.2/mne/io/eyelink/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eyelink/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6246 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/eyelink/tests/test_eyelink.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.619075 mne-1.4.2/mne/io/fieldtrip/
+-rw-r--r--   0 larsoner   (501) staff       (20)      247 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fieldtrip/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6673 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fieldtrip/fieldtrip.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.619497 mne-1.4.2/mne/io/fieldtrip/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)      158 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/fieldtrip/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6446 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fieldtrip/tests/helpers.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12151 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fieldtrip/tests/test_fieldtrip.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12204 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fieldtrip/utils.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.619850 mne-1.4.2/mne/io/fiff/
+-rw-r--r--   0 larsoner   (501) staff       (20)       79 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/fiff/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20787 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fiff/raw.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.620108 mne-1.4.2/mne/io/fiff/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/fiff/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    77607 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fiff/tests/test_raw_fiff.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.620606 mne-1.4.2/mne/io/fil/
+-rw-r--r--   0 larsoner   (501) staff       (20)      105 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fil/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10467 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fil/fil.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4501 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fil/sensors.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.620736 mne-1.4.2/mne/io/fil/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     4270 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/fil/tests/test_fil.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.621031 mne-1.4.2/mne/io/hitachi/
+-rw-r--r--   0 larsoner   (501) staff       (20)      156 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/hitachi/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12655 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/hitachi/hitachi.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.621192 mne-1.4.2/mne/io/hitachi/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)    59466 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/hitachi/tests/test_hitachi.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.621892 mne-1.4.2/mne/io/kit/
+-rw-r--r--   0 larsoner   (501) staff       (20)      188 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/kit/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9156 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/constants.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7774 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    36969 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/kit.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.622339 mne-1.4.2/mne/io/kit/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)       68 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      984 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/tests/test_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16867 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/kit/tests/test_kit.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4398 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/matrix.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   114631 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/meas_info.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.622724 mne-1.4.2/mne/io/nedf/
+-rw-r--r--   0 larsoner   (501) staff       (20)      162 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/nedf/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7783 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nedf/nedf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.623112 mne-1.4.2/mne/io/nedf/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        1 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/nedf/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4467 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nedf/tests/test_nedf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.623469 mne-1.4.2/mne/io/nicolet/
+-rw-r--r--   0 larsoner   (501) staff       (20)      165 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/nicolet/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6568 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nicolet/nicolet.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.623683 mne-1.4.2/mne/io/nicolet/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:56.000000 mne-1.4.2/mne/io/nicolet/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      750 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nicolet/tests/test_nicolet.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.623946 mne-1.4.2/mne/io/nihon/
+-rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/nihon/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18051 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nihon/nihon.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.624117 mne-1.4.2/mne/io/nihon/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     3453 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nihon/tests/test_nihon.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.624737 mne-1.4.2/mne/io/nirx/
+-rw-r--r--   0 larsoner   (501) staff       (20)      146 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/nirx/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3950 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nirx/_localized_abbr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22266 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nirx/nirx.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.625002 mne-1.4.2/mne/io/nirx/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.2/mne/io/nirx/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26253 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/nirx/tests/test_nirx.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11246 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/open.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.625428 mne-1.4.2/mne/io/persyst/
+-rw-r--r--   0 larsoner   (501) staff       (20)      149 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/persyst/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16850 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/persyst/persyst.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.625682 mne-1.4.2/mne/io/persyst/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/persyst/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8750 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/persyst/tests/test_persyst.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    46005 2023-06-06 14:38:39.000000 mne-1.4.2/mne/io/pick.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11702 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/proc_history.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    38454 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/proj.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    24159 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/reference.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.625949 mne-1.4.2/mne/io/snirf/
+-rw-r--r--   0 larsoner   (501) staff       (20)      149 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/snirf/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22347 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/snirf/_snirf.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.626199 mne-1.4.2/mne/io/snirf/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.2/mne/io/snirf/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15517 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/snirf/tests/test_snirf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18102 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tag.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.628676 mne-1.4.2/mne/io/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)       71 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1892 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_apply_function.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4249 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_compensator.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14879 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_constants.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    40085 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_meas_info.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    28743 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_pick.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1403 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_proc_history.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    36373 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2891 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_read_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    32089 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_reference.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      917 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_show_fiff.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      578 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1720 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_what.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      782 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tests/test_write.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4694 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/tree.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11601 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2128 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/what.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17887 2023-06-05 14:01:41.000000 mne-1.4.2/mne/io/write.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   100868 2023-06-05 14:01:41.000000 mne-1.4.2/mne/label.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.629852 mne-1.4.2/mne/minimum_norm/
+-rw-r--r--   0 larsoner   (501) staff       (20)      724 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7301 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/_eloreta.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    72953 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16454 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/resolution_matrix.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12826 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/spatial_resolution.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.631034 mne-1.4.2/mne/minimum_norm/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/minimum_norm/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    62883 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/tests/test_inverse.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9806 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/tests/test_resolution_matrix.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5905 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/tests/test_resolution_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1514 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/tests/test_snr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8495 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/tests/test_time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    30779 2023-06-05 14:01:41.000000 mne-1.4.2/mne/minimum_norm/time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2926 2023-06-05 14:01:41.000000 mne-1.4.2/mne/misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    58424 2023-06-05 14:01:41.000000 mne-1.4.2/mne/morph.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9169 2023-06-05 14:01:41.000000 mne-1.4.2/mne/morph_map.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4848 2023-06-05 14:01:41.000000 mne-1.4.2/mne/parallel.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.635331 mne-1.4.2/mne/preprocessing/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1716 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11302 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/_csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2963 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/_css.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20851 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/_fine_cal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6277 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/_peak_finder.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13215 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/_regress.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11365 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/annotate_amplitude.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1139 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/annotate_nan.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22725 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/artifact_detection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1549 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/bads.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5139 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ctps_.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15571 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ecg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9572 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/eog.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.635863 mne-1.4.2/mne/preprocessing/eyetracking/
+-rw-r--r--   0 larsoner   (501) staff       (20)      186 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/eyetracking/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5475 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/eyetracking/eyetracking.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3368 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/hfc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   127544 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ica.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.636297 mne-1.4.2/mne/preprocessing/ieeg/
+-rw-r--r--   0 larsoner   (501) staff       (20)      242 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ieeg/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7434 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ieeg/_projection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8858 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ieeg/_volume.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.636592 mne-1.4.2/mne/preprocessing/ieeg/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     7620 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ieeg/tests/test_projection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4713 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ieeg/tests/test_volume.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11695 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/infomax_.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8651 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/interpolate.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6448 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/maxfilter.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   111776 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/maxwell.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.637464 mne-1.4.2/mne/preprocessing/nirs/
+-rw-r--r--   0 larsoner   (501) staff       (20)      711 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3697 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/_beer_lambert_law.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1719 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/_optical_density.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1861 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/_scalp_coupling_index.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5020 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/_tddr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11536 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/nirs.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.638209 mne-1.4.2/mne/preprocessing/nirs/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     3525 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/tests/test_beer_lambert_law.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20195 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/tests/test_nirs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1991 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/tests/test_optical_density.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2579 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/tests/test_scalp_coupling_index.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1989 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/nirs/tests/test_temporal_derivative_distribution_repair.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5040 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/otp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4251 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/realign.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15699 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/ssp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4375 2023-06-06 14:38:39.000000 mne-1.4.2/mne/preprocessing/stim.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.641763 mne-1.4.2/mne/preprocessing/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/preprocessing/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16015 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_annotate_amplitude.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1554 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_annotate_nan.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9840 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_artifact_detection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8921 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1697 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_css.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2914 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_ctps.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3481 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_ecg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6953 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_eeglab_infomax.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1103 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_eog.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6236 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_fine_cal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5495 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_hfc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    61957 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_ica.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6022 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_infomax.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7517 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_interpolate.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    71419 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_maxwell.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3770 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_otp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1168 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_peak_finder.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5050 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_realign.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6864 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_regress.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9007 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_ssp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4074 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_stim.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12753 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/tests/test_xdawn.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    24815 2023-06-05 14:01:41.000000 mne-1.4.2/mne/preprocessing/xdawn.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16185 2023-06-06 14:38:39.000000 mne-1.4.2/mne/proj.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17313 2023-06-05 14:01:41.000000 mne-1.4.2/mne/rank.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.642170 mne-1.4.2/mne/report/
+-rw-r--r--   0 larsoner   (501) staff       (20)       56 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/__init__.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.644513 mne-1.4.2/mne/report/js_and_css/
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.645326 mne-1.4.2/mne/report/js_and_css/bootstrap-icons/
+-rw-r--r--   0 larsoner   (501) staff       (20)   186639 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-icons/bootstrap-icons.mne.min.css
+-rw-r--r--   0 larsoner   (501) staff       (20)     1483 2023-06-05 14:01:41.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-icons/gen_css_for_mne.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.646318 mne-1.4.2/mne/report/js_and_css/bootstrap-table/
+-rw-r--r--   0 larsoner   (501) staff       (20)    15127 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table-copy-rows.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)    28095 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table-export.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)     9246 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.css
+-rw-r--r--   0 larsoner   (501) staff       (20)   121976 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)    77394 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap-table/tableExport.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)    78871 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap.bundle.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)   162764 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/bootstrap.min.css
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.647014 mne-1.4.2/mne/report/js_and_css/highlightjs/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1193 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/highlightjs/atom-one-dark-reasonable.min.css
+-rw-r--r--   0 larsoner   (501) staff       (20)      856 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/highlightjs/atom-one-light.min.css
+-rw-r--r--   0 larsoner   (501) staff       (20)     1147 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/highlightjs/default.min.css
+-rw-r--r--   0 larsoner   (501) staff       (20)   132027 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/highlightjs/highlight.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)    89501 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/jquery-3.6.0.min.js
+-rw-r--r--   0 larsoner   (501) staff       (20)     8008 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/report.js
+-rw-r--r--   0 larsoner   (501) staff       (20)      257 2022-11-28 17:38:21.000000 mne-1.4.2/mne/report/js_and_css/report.sass
+-rw-r--r--   0 larsoner   (501) staff       (20)   143136 2023-06-06 14:38:39.000000 mne-1.4.2/mne/report/report.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.647298 mne-1.4.2/mne/report/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)    38595 2023-06-05 14:01:41.000000 mne-1.4.2/mne/report/tests/test_report.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.649397 mne-1.4.2/mne/simulation/
+-rw-r--r--   0 larsoner   (501) staff       (20)      270 2023-04-21 22:27:15.000000 mne-1.4.2/mne/simulation/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      419 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5498 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/evoked.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.649751 mne-1.4.2/mne/simulation/metrics/
+-rw-r--r--   0 larsoner   (501) staff       (20)      348 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/metrics/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17520 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/metrics/metrics.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.650022 mne-1.4.2/mne/simulation/metrics/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:21.000000 mne-1.4.2/mne/simulation/metrics/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9371 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/metrics/tests/test_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    30788 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21249 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/source.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.650753 mne-1.4.2/mne/simulation/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/simulation/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7263 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/tests/test_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1782 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/tests/test_metrics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22779 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/tests/test_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15089 2023-06-05 14:01:41.000000 mne-1.4.2/mne/simulation/tests/test_source.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   131857 2023-06-05 14:01:41.000000 mne-1.4.2/mne/source_estimate.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   121184 2023-06-05 14:01:41.000000 mne-1.4.2/mne/source_space.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.652372 mne-1.4.2/mne/stats/
+-rw-r--r--   0 larsoner   (501) staff       (20)      662 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4702 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/_adjacency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    60183 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/cluster_level.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2997 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/multi_comp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14482 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/parametric.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6035 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/permutations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17689 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/regression.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.653510 mne-1.4.2/mne/stats/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/stats/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1309 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/tests/test_adjacency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    30632 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/tests/test_cluster_level.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1952 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/tests/test_multi_comp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5963 2023-06-05 14:01:41.000000 mne-1.4.2/mne/stats/tests/test_parametric.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2760 2023-06-06 14:38:39.000000 mne-1.4.2/mne/stats/tests/test_permutations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5558 2023-06-06 14:38:39.000000 mne-1.4.2/mne/stats/tests/test_regression.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    80420 2023-06-06 14:38:39.000000 mne-1.4.2/mne/surface.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.660002 mne-1.4.2/mne/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.2/mne/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    65393 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_annotations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22891 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_bem.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    31426 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_chpi.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22434 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    35365 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_cov.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1952 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_defaults.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21338 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_dipole.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11111 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_docstring_parameters.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   170384 2023-06-06 14:38:39.000000 mne-1.4.2/mne/tests/test_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    23810 2023-06-06 14:38:39.000000 mne-1.4.2/mne/tests/test_event.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    35726 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    36094 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_filter.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10356 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_freesurfer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1864 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_import_nesting.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    43386 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_label.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2778 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_line_endings.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      362 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    43508 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_morph.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2165 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_morph_map.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4672 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_ola.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1121 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_parallel.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21664 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_proj.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11588 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_rank.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1953 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_read_vectorview_selection.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    75965 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_source_estimate.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    39370 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_source_space.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    19680 2023-06-06 14:38:39.000000 mne-1.4.2/mne/tests/test_surface.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22045 2023-06-05 14:01:41.000000 mne-1.4.2/mne/tests/test_transforms.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.661802 mne-1.4.2/mne/time_frequency/
+-rw-r--r--   0 larsoner   (501) staff       (20)      746 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6811 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/_stft.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9665 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/_stockwell.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2335 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/ar.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    50272 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17488 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/multitaper.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7629 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/psd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    47024 2023-06-06 14:38:39.000000 mne-1.4.2/mne/time_frequency/spectrum.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.663522 mne-1.4.2/mne/time_frequency/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/time_frequency/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1805 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_ar.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21280 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_csd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2943 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_multitaper.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8129 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_psd.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12507 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_spectrum.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2204 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_stft.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5365 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_stockwell.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    50185 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tests/test_tfr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   110913 2023-06-05 14:01:41.000000 mne-1.4.2/mne/time_frequency/tfr.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    66973 2023-06-05 14:01:41.000000 mne-1.4.2/mne/transforms.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.668001 mne-1.4.2/mne/utils/
+-rw-r--r--   0 larsoner   (501) staff       (20)     4443 2023-06-06 14:38:39.000000 mne-1.4.2/mne/utils/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3035 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/_bunch.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17017 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/_logging.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13569 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/_testing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    40479 2023-06-06 14:38:39.000000 mne-1.4.2/mne/utils/check.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26682 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/config.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3772 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/dataframe.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   174485 2023-06-06 14:38:39.000000 mne-1.4.2/mne/utils/docs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      583 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/fetching.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6450 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/linalg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15198 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26420 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/mixin.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    38080 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/numerics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6724 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/progressbar.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2732 2023-06-06 14:38:39.000000 mne-1.4.2/mne/utils/spectrum.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.669720 mne-1.4.2/mne/utils/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)      643 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_bunch.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11942 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_check.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4679 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_config.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5783 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_docs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3668 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_linalg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8439 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_logging.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4102 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-11-28 17:38:12.000000 mne-1.4.2/mne/utils/tests/test_mixin.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21290 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_numerics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4324 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_progressbar.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1569 2023-06-05 14:01:41.000000 mne-1.4.2/mne/utils/tests/test_testing.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.675882 mne-1.4.2/mne/viz/
+-rw-r--r--   0 larsoner   (501) staff       (20)   144063 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_3d.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5679 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_3d_overlay.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2141 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/__init__.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.677776 mne-1.4.2/mne/viz/_brain/
+-rw-r--r--   0 larsoner   (501) staff       (20)      510 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   156784 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/_brain.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5432 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/_linkviewer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4034 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/_scraper.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3714 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/callback.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6463 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/colormap.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6322 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/surface.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.678096 mne-1.4.2/mne/viz/_brain/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)    46475 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/tests/test_brain.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5542 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/tests/test_notebook.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2455 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_brain/view.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7020 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_dipole.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    31796 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_figure.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   105679 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_mpl_figure.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9716 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_proj.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2687 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/_scraper.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.680688 mne-1.4.2/mne/viz/backends/
+-rw-r--r--   0 larsoner   (501) staff       (20)       53 2022-11-28 17:38:12.000000 mne-1.4.2/mne/viz/backends/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    37818 2023-06-05 17:39:02.000000 mne-1.4.2/mne/viz/backends/_abstract.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    50094 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/_notebook.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    47031 2023-06-06 14:38:41.000000 mne-1.4.2/mne/viz/backends/_pyvista.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    60304 2023-06-06 14:38:41.000000 mne-1.4.2/mne/viz/backends/_qt.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15557 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11950 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/renderer.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.681547 mne-1.4.2/mne/viz/backends/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)     1164 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/tests/_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4553 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/tests/test_abstract.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7437 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/tests/test_renderer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3869 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/backends/tests/test_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15169 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/circle.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1633 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/conftest.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    42586 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   117627 2023-06-06 14:38:39.000000 mne-1.4.2/mne/viz/evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    44556 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/ica.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    54351 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2847 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/montage.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    20840 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/raw.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.685146 mne-1.4.2/mne/viz/tests/
+-rw-r--r--   0 larsoner   (501) staff       (20)        0 2022-05-20 17:14:57.000000 mne-1.4.2/mne/viz/tests/__init__.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    38878 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_3d.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5336 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_3d_mpl.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1054 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_circle.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18499 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    23911 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      366 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_figure.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    17568 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_ica.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11878 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_misc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2757 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_montage.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2235 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_proj.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    41544 2023-06-06 14:38:39.000000 mne-1.4.2/mne/viz/tests/test_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     1003 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_scraper.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13267 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_topo.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    33336 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_topomap.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6990 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/tests/test_utils.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    40149 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/topo.py
+-rw-r--r--   0 larsoner   (501) staff       (20)   126112 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/topomap.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    99194 2023-06-05 14:01:41.000000 mne-1.4.2/mne/viz/utils.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.528025 mne-1.4.2/mne.egg-info/
+-rw-r--r--   0 larsoner   (501) staff       (20)     6944 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/PKG-INFO
+-rw-r--r--   0 larsoner   (501) staff       (20)    36048 2023-06-06 14:44:59.000000 mne-1.4.2/mne.egg-info/SOURCES.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)        1 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/dependency_links.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)       48 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/entry_points.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)        1 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/not-zip-safe
+-rw-r--r--   0 larsoner   (501) staff       (20)      434 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/requires.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)        4 2023-06-06 14:44:58.000000 mne-1.4.2/mne.egg-info/top_level.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)     1554 2023-06-05 14:01:41.000000 mne-1.4.2/pyproject.toml
+-rw-r--r--   0 larsoner   (501) staff       (20)      730 2023-06-06 14:39:18.000000 mne-1.4.2/requirements.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      188 2023-06-05 14:01:41.000000 mne-1.4.2/requirements_base.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      530 2023-06-05 14:01:41.000000 mne-1.4.2/requirements_doc.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)       75 2022-11-28 17:38:21.000000 mne-1.4.2/requirements_hdf5.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      223 2023-06-05 14:01:41.000000 mne-1.4.2/requirements_testing.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)      173 2023-06-05 14:01:41.000000 mne-1.4.2/requirements_testing_extra.txt
+-rw-r--r--   0 larsoner   (501) staff       (20)       38 2023-06-06 14:44:59.701376 mne-1.4.2/setup.cfg
+-rw-r--r--   0 larsoner   (501) staff       (20)     5491 2023-06-06 14:41:28.000000 mne-1.4.2/setup.py
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.685282 mne-1.4.2/tutorials/
+-rw-r--r--   0 larsoner   (501) staff       (20)      856 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.685913 mne-1.4.2/tutorials/clinical/
+-rw-r--r--   0 larsoner   (501) staff       (20)     8652 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/clinical/20_seeg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7944 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/clinical/30_ecog.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11308 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/clinical/60_sleep.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      849 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/clinical/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.687291 mne-1.4.2/tutorials/epochs/
+-rw-r--r--   0 larsoner   (501) staff       (20)    17931 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/10_epochs_overview.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11211 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/15_baseline_regression.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12231 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/20_visualize_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6895 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/30_epochs_metadata.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    18668 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/40_autogenerate_metadata.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6295 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/50_epochs_to_data_frame.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5100 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/epochs/60_make_fixed_length_epochs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      169 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/epochs/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.688131 mne-1.4.2/tutorials/evoked/
+-rw-r--r--   0 larsoner   (501) staff       (20)    15451 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/evoked/10_evoked_overview.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11855 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/evoked/20_visualize_evoked.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    28275 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/evoked/30_eeg_erp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2327 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/evoked/40_whitened.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      183 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/evoked/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.689401 mne-1.4.2/tutorials/forward/
+-rw-r--r--   0 larsoner   (501) staff       (20)     5741 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/10_background_freesurfer.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16105 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/20_source_alignment.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4183 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/25_automated_coreg.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10233 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/30_forward.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5278 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/35_eeg_no_mri.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21487 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/50_background_freesurfer_mne.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14059 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/80_fix_bem_in_blender.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7966 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/forward/90_compute_covariance.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      196 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/forward/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.690570 mne-1.4.2/tutorials/intro/
+-rw-r--r--   0 larsoner   (501) staff       (20)    18252 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/10_overview.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4034 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/15_inplace.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13980 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/20_events_from_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7745 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/30_info.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13146 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/40_sensor_locations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9643 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/50_configure_mne.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    27642 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/intro/70_report.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      321 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/intro/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.692398 mne-1.4.2/tutorials/inverse/
+-rw-r--r--   0 larsoner   (501) staff       (20)     9293 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/10_stc_class.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4775 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/20_dipole_fit.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4895 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/30_mne_dspm_loreta.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9462 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/35_dipole_orientations.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3614 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/40_mne_fixed_free.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12118 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/50_beamformer_lcmv.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7664 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/60_visualize_stc.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6646 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/70_eeg_mri_coords.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6531 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/80_brainstorm_phantom_elekta.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3862 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/85_brainstorm_phantom_ctf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     2505 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/inverse/90_phantom_4DBTi.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      145 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/inverse/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.693206 mne-1.4.2/tutorials/io/
+-rw-r--r--   0 larsoner   (501) staff       (20)    13012 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/io/10_reading_meg_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9041 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/io/20_reading_eeg_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    10187 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/io/30_reading_fnirs_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    14167 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/io/60_ctf_bst_auditory.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7858 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/io/70_reading_eyetracking_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      218 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/io/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.693772 mne-1.4.2/tutorials/machine-learning/
+-rw-r--r--   0 larsoner   (501) staff       (20)    13605 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/machine-learning/30_strf.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16655 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/machine-learning/50_decoding.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      171 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/machine-learning/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.696618 mne-1.4.2/tutorials/preprocessing/
+-rw-r--r--   0 larsoner   (501) staff       (20)    11133 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/10_preprocessing_overview.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12395 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/15_handling_bad_channels.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13749 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/20_rejecting_bad_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    46385 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/25_background_filtering.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    13464 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/30_filtering_resampling.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9913 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/35_artifact_correction_regression.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    30001 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/40_artifact_correction_ica.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    21535 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/45_projectors_background.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    22828 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/50_artifact_correction_ssp.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11436 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/55_setting_eeg_reference.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3736 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/59_head_positions.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    16567 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/60_maxwell_filtering_sss.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    12305 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/70_fnirs_processing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     8828 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/80_opm_processing.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     3866 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/preprocessing/90_eyetracking_data.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      150 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/preprocessing/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.697590 mne-1.4.2/tutorials/raw/
+-rw-r--r--   0 larsoner   (501) staff       (20)       22 2022-11-28 17:38:12.000000 mne-1.4.2/tutorials/raw/.gitignore
+-rw-r--r--   0 larsoner   (501) staff       (20)    25952 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/raw/10_raw_overview.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7984 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/raw/20_event_arrays.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11027 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/raw/30_annotate_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9168 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/raw/40_visualize_raw.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      242 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/raw/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.698161 mne-1.4.2/tutorials/simulation/
+-rw-r--r--   0 larsoner   (501) staff       (20)     9124 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/simulation/10_array_objs.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     6182 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/simulation/70_point_spread.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11401 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/simulation/80_dics.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      177 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/simulation/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.699207 mne-1.4.2/tutorials/stats-sensor-space/
+-rw-r--r--   0 larsoner   (501) staff       (20)    29116 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/10_background_stats.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     5491 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/20_erp_stats.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9511 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/40_cluster_1samp_time_freq.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4894 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/50_cluster_between_time_freq.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     9833 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/70_cluster_rmANOVA_time_freq.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    15038 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-sensor-space/75_cluster_ftest_spatiotemporal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      160 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/stats-sensor-space/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.700025 mne-1.4.2/tutorials/stats-source-space/
+-rw-r--r--   0 larsoner   (501) staff       (20)     9178 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-source-space/20_cluster_1samp_spatiotemporal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     4276 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-source-space/30_cluster_ftest_spatiotemporal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    11262 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/stats-source-space/60_cluster_rmANOVA_spatiotemporal.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      162 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/stats-source-space/README.txt
+drwxr-xr-x   0 larsoner   (501) staff       (20)        0 2023-06-06 14:44:59.700821 mne-1.4.2/tutorials/time-freq/
+-rw-r--r--   0 larsoner   (501) staff       (20)     8044 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/time-freq/10_spectrum_class.py
+-rw-r--r--   0 larsoner   (501) staff       (20)     7801 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/time-freq/20_sensors_time_frequency.py
+-rw-r--r--   0 larsoner   (501) staff       (20)    26579 2023-06-05 14:01:41.000000 mne-1.4.2/tutorials/time-freq/50_ssvep.py
+-rw-r--r--   0 larsoner   (501) staff       (20)      128 2022-11-28 17:38:21.000000 mne-1.4.2/tutorials/time-freq/README.txt
```

### Comparing `mne-1.4.1/.circleci/config.yml` & `mne-1.4.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/CODEOWNERS` & `mne-1.4.2/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `mne-1.4.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/ISSUE_TEMPLATE/documentation.yml` & `mne-1.4.2/.github/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `mne-1.4.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/config.yml` & `mne-1.4.2/.github/config.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/workflows/circle_artifacts.yml` & `mne-1.4.2/.github/workflows/circle_artifacts.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/workflows/codeql-analysis.yml` & `mne-1.4.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.github/workflows/tests.yml` & `mne-1.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/.gitignore` & `mne-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/LICENSE.txt` & `mne-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/MANIFEST.in` & `mne-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/PKG-INFO` & `mne-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne
-Version: 1.4.1
+Version: 1.4.2
 Summary: MNE-Python project for MEG and EEG data analysis.
 Home-page: https://mne.tools/dev/
 Download-URL: http://github.com/mne-tools/mne-python
 Maintainer: Alexandre Gramfort
 Maintainer-email: alexandre.gramfort@inria.fr
 License: BSD-3-Clause
 Project-URL: Homepage, https://mne.tools/
```

### Comparing `mne-1.4.1/README.rst` & `mne-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/SECURITY.md` & `mne-1.4.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/README.txt` & `mne-1.4.2/examples/README.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/datasets/brainstorm_data.py` & `mne-1.4.2/examples/datasets/brainstorm_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/datasets/hf_sef_data.py` & `mne-1.4.2/examples/datasets/hf_sef_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/datasets/limo_data.py` & `mne-1.4.2/examples/datasets/limo_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/datasets/opm_data.py` & `mne-1.4.2/examples/datasets/opm_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/datasets/spm_faces_dataset_sgskip.py` & `mne-1.4.2/examples/datasets/spm_faces_dataset_sgskip.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_csp_eeg.py` & `mne-1.4.2/examples/decoding/decoding_csp_eeg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_csp_timefreq.py` & `mne-1.4.2/examples/decoding/decoding_csp_timefreq.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_rsa_sgskip.py` & `mne-1.4.2/examples/decoding/decoding_rsa_sgskip.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_spatio_temporal_source.py` & `mne-1.4.2/examples/decoding/decoding_spatio_temporal_source.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_spoc_CMC.py` & `mne-1.4.2/examples/decoding/decoding_spoc_CMC.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_time_generalization_conditions.py` & `mne-1.4.2/examples/decoding/decoding_time_generalization_conditions.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_unsupervised_spatial_filter.py` & `mne-1.4.2/examples/decoding/decoding_unsupervised_spatial_filter.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/decoding_xdawn_eeg.py` & `mne-1.4.2/examples/decoding/decoding_xdawn_eeg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/ems_filtering.py` & `mne-1.4.2/examples/decoding/ems_filtering.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/linear_model_patterns.py` & `mne-1.4.2/examples/decoding/linear_model_patterns.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/receptive_field_mtrf.py` & `mne-1.4.2/examples/decoding/receptive_field_mtrf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/decoding/ssd_spatial_filters.py` & `mne-1.4.2/examples/decoding/ssd_spatial_filters.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/forward/forward_sensitivity_maps.py` & `mne-1.4.2/examples/forward/forward_sensitivity_maps.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/forward/left_cerebellum_volume_source.py` & `mne-1.4.2/examples/forward/left_cerebellum_volume_source.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/forward/source_space_morphing.py` & `mne-1.4.2/examples/forward/source_space_morphing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/compute_mne_inverse_epochs_in_label.py` & `mne-1.4.2/examples/inverse/compute_mne_inverse_epochs_in_label.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/compute_mne_inverse_raw_in_label.py` & `mne-1.4.2/examples/inverse/compute_mne_inverse_raw_in_label.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/compute_mne_inverse_volume.py` & `mne-1.4.2/examples/inverse/compute_mne_inverse_volume.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/custom_inverse_solver.py` & `mne-1.4.2/examples/inverse/custom_inverse_solver.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/dics_epochs.py` & `mne-1.4.2/examples/inverse/dics_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/dics_source_power.py` & `mne-1.4.2/examples/inverse/dics_source_power.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/evoked_ers_source_power.py` & `mne-1.4.2/examples/inverse/evoked_ers_source_power.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/gamma_map_inverse.py` & `mne-1.4.2/examples/inverse/gamma_map_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/label_activation_from_stc.py` & `mne-1.4.2/examples/inverse/label_activation_from_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/label_from_stc.py` & `mne-1.4.2/examples/inverse/label_from_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/label_source_activations.py` & `mne-1.4.2/examples/inverse/label_source_activations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/mixed_norm_inverse.py` & `mne-1.4.2/examples/inverse/mixed_norm_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/mixed_source_space_inverse.py` & `mne-1.4.2/examples/inverse/mixed_source_space_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/mne_cov_power.py` & `mne-1.4.2/examples/inverse/mne_cov_power.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/morph_surface_stc.py` & `mne-1.4.2/examples/inverse/morph_surface_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/morph_volume_stc.py` & `mne-1.4.2/examples/inverse/morph_volume_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/multi_dipole_model.py` & `mne-1.4.2/examples/inverse/multi_dipole_model.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/multidict_reweighted_tfmxne.py` & `mne-1.4.2/examples/inverse/multidict_reweighted_tfmxne.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/psf_ctf_label_leakage.py` & `mne-1.4.2/examples/inverse/psf_ctf_label_leakage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/psf_ctf_vertices.py` & `mne-1.4.2/examples/inverse/psf_ctf_vertices.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/psf_ctf_vertices_lcmv.py` & `mne-1.4.2/examples/inverse/psf_ctf_vertices_lcmv.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/psf_volume.py` & `mne-1.4.2/examples/inverse/psf_volume.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/rap_music.py` & `mne-1.4.2/examples/inverse/rap_music.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/read_inverse.py` & `mne-1.4.2/examples/inverse/read_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/read_stc.py` & `mne-1.4.2/examples/inverse/read_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/resolution_metrics.py` & `mne-1.4.2/examples/inverse/resolution_metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/resolution_metrics_eegmeg.py` & `mne-1.4.2/examples/inverse/resolution_metrics_eegmeg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/snr_estimate.py` & `mne-1.4.2/examples/inverse/snr_estimate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/source_space_snr.py` & `mne-1.4.2/examples/inverse/source_space_snr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/time_frequency_mixed_norm_inverse.py` & `mne-1.4.2/examples/inverse/time_frequency_mixed_norm_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/trap_music.py` & `mne-1.4.2/examples/inverse/trap_music.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/inverse/vector_mne_solution.py` & `mne-1.4.2/examples/inverse/vector_mne_solution.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/io/elekta_epochs.py` & `mne-1.4.2/examples/io/elekta_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/io/read_neo_format.py` & `mne-1.4.2/examples/io/read_neo_format.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/io/read_noise_covariance_matrix.py` & `mne-1.4.2/examples/io/read_noise_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/io/read_xdf.py` & `mne-1.4.2/examples/io/read_xdf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/README.txt` & `mne-1.4.2/examples/preprocessing/README.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/contralateral_referencing.py` & `mne-1.4.2/examples/preprocessing/contralateral_referencing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/css.py` & `mne-1.4.2/examples/preprocessing/css.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/define_target_events.py` & `mne-1.4.2/examples/preprocessing/define_target_events.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/eeg_bridging.py` & `mne-1.4.2/examples/preprocessing/eeg_bridging.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/eeg_csd.py` & `mne-1.4.2/examples/preprocessing/eeg_csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/eog_artifact_histogram.py` & `mne-1.4.2/examples/preprocessing/eog_artifact_histogram.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/eog_regression.py` & `mne-1.4.2/examples/preprocessing/eog_regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/find_ref_artifacts.py` & `mne-1.4.2/examples/preprocessing/find_ref_artifacts.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/fnirs_artifact_removal.py` & `mne-1.4.2/examples/preprocessing/fnirs_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/ica_comparison.py` & `mne-1.4.2/examples/preprocessing/ica_comparison.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/interpolate_bad_channels.py` & `mne-1.4.2/examples/preprocessing/interpolate_bad_channels.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/movement_compensation.py` & `mne-1.4.2/examples/preprocessing/movement_compensation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/movement_detection.py` & `mne-1.4.2/examples/preprocessing/movement_detection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/muscle_detection.py` & `mne-1.4.2/examples/preprocessing/muscle_detection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/muscle_ica.py` & `mne-1.4.2/examples/preprocessing/muscle_ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/otp.py` & `mne-1.4.2/examples/preprocessing/otp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/shift_evoked.py` & `mne-1.4.2/examples/preprocessing/shift_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/virtual_evoked.py` & `mne-1.4.2/examples/preprocessing/virtual_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/preprocessing/xdawn_denoising.py` & `mne-1.4.2/examples/preprocessing/xdawn_denoising.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/simulation/plot_stc_metrics.py` & `mne-1.4.2/examples/simulation/plot_stc_metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/simulation/simulate_evoked_data.py` & `mne-1.4.2/examples/simulation/simulate_evoked_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/simulation/simulate_raw_data.py` & `mne-1.4.2/examples/simulation/simulate_raw_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/simulation/simulated_raw_data_using_subject_anatomy.py` & `mne-1.4.2/examples/simulation/simulated_raw_data_using_subject_anatomy.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/simulation/source_simulator.py` & `mne-1.4.2/examples/simulation/source_simulator.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/stats/cluster_stats_evoked.py` & `mne-1.4.2/examples/stats/cluster_stats_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/stats/fdr_stats_evoked.py` & `mne-1.4.2/examples/stats/fdr_stats_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/stats/linear_regression_raw.py` & `mne-1.4.2/examples/stats/linear_regression_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/stats/sensor_permutation_test.py` & `mne-1.4.2/examples/stats/sensor_permutation_test.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/stats/sensor_regression.py` & `mne-1.4.2/examples/stats/sensor_regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/compute_csd.py` & `mne-1.4.2/examples/time_frequency/compute_csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/compute_source_psd_epochs.py` & `mne-1.4.2/examples/time_frequency/compute_source_psd_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/source_label_time_frequency.py` & `mne-1.4.2/examples/time_frequency/source_label_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/source_power_spectrum.py` & `mne-1.4.2/examples/time_frequency/source_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/source_power_spectrum_opm.py` & `mne-1.4.2/examples/time_frequency/source_power_spectrum_opm.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/source_space_time_frequency.py` & `mne-1.4.2/examples/time_frequency/source_space_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/temporal_whitening.py` & `mne-1.4.2/examples/time_frequency/temporal_whitening.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/time_frequency_erds.py` & `mne-1.4.2/examples/time_frequency/time_frequency_erds.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/time_frequency_global_field_power.py` & `mne-1.4.2/examples/time_frequency/time_frequency_global_field_power.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/time_frequency/time_frequency_simulated.py` & `mne-1.4.2/examples/time_frequency/time_frequency_simulated.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/3d_to_2d.py` & `mne-1.4.2/examples/visualization/3d_to_2d.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/brain.py` & `mne-1.4.2/examples/visualization/brain.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/channel_epochs_image.py` & `mne-1.4.2/examples/visualization/channel_epochs_image.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/eeg_on_scalp.py` & `mne-1.4.2/examples/visualization/eeg_on_scalp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/evoked_arrowmap.py` & `mne-1.4.2/examples/visualization/evoked_arrowmap.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/evoked_topomap.py` & `mne-1.4.2/examples/visualization/evoked_topomap.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/evoked_whitening.py` & `mne-1.4.2/examples/visualization/evoked_whitening.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/meg_sensors.py` & `mne-1.4.2/examples/visualization/meg_sensors.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/mne_helmet.py` & `mne-1.4.2/examples/visualization/mne_helmet.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/montage_sgskip.py` & `mne-1.4.2/examples/visualization/montage_sgskip.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/parcellation.py` & `mne-1.4.2/examples/visualization/parcellation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/publication_figure.py` & `mne-1.4.2/examples/visualization/publication_figure.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/roi_erpimage_by_rt.py` & `mne-1.4.2/examples/visualization/roi_erpimage_by_rt.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/sensor_noise_level.py` & `mne-1.4.2/examples/visualization/sensor_noise_level.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/ssp_projs_sensitivity_map.py` & `mne-1.4.2/examples/visualization/ssp_projs_sensitivity_map.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/topo_compare_conditions.py` & `mne-1.4.2/examples/visualization/topo_compare_conditions.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/topo_customized.py` & `mne-1.4.2/examples/visualization/topo_customized.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/examples/visualization/xhemi.py` & `mne-1.4.2/examples/visualization/xhemi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/__init__.py` & `mne-1.4.2/mne/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/_freesurfer.py` & `mne-1.4.2/mne/_freesurfer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/_ola.py` & `mne-1.4.2/mne/_ola.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/annotations.py` & `mne-1.4.2/mne/annotations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/baseline.py` & `mne-1.4.2/mne/baseline.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/_compute_beamformer.py` & `mne-1.4.2/mne/beamformer/_compute_beamformer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/_dics.py` & `mne-1.4.2/mne/beamformer/_dics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/_lcmv.py` & `mne-1.4.2/mne/beamformer/_lcmv.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/_rap_music.py` & `mne-1.4.2/mne/beamformer/_rap_music.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/resolution_matrix.py` & `mne-1.4.2/mne/beamformer/resolution_matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/tests/test_dics.py` & `mne-1.4.2/mne/beamformer/tests/test_dics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/tests/test_external.py` & `mne-1.4.2/mne/beamformer/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/tests/test_lcmv.py` & `mne-1.4.2/mne/beamformer/tests/test_lcmv.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/tests/test_rap_music.py` & `mne-1.4.2/mne/beamformer/tests/test_rap_music.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/beamformer/tests/test_resolution_matrix.py` & `mne-1.4.2/mne/beamformer/tests/test_resolution_matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/bem.py` & `mne-1.4.2/mne/bem.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/__init__.py` & `mne-1.4.2/mne/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/_dig_montage_utils.py` & `mne-1.4.2/mne/channels/_dig_montage_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/_standard_montage_utils.py` & `mne-1.4.2/mne/channels/_standard_montage_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/channels.py` & `mne-1.4.2/mne/channels/channels.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/CTF-275.lout` & `mne-1.4.2/mne/channels/data/layouts/CTF-275.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/CTF151.lay` & `mne-1.4.2/mne/channels/data/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/CTF275.lay` & `mne-1.4.2/mne/channels/data/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/EEG1005.lay` & `mne-1.4.2/mne/channels/data/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/EGI256.lout` & `mne-1.4.2/mne/channels/data/layouts/EGI256.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/GeodesicHeadWeb-130.lout` & `mne-1.4.2/mne/channels/data/layouts/GeodesicHeadWeb-130.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/GeodesicHeadWeb-280.lout` & `mne-1.4.2/mne/channels/data/layouts/GeodesicHeadWeb-280.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-125.lout` & `mne-1.4.2/mne/channels/data/layouts/KIT-125.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-157.lout` & `mne-1.4.2/mne/channels/data/layouts/KIT-157.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-160.lay` & `mne-1.4.2/mne/channels/data/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-AD.lout` & `mne-1.4.2/mne/channels/data/layouts/KIT-AD.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-AS-2008.lout` & `mne-1.4.2/mne/channels/data/layouts/KIT-AS-2008.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/KIT-UMD-3.lout` & `mne-1.4.2/mne/channels/data/layouts/KIT-UMD-3.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/Neuromag_122.lout` & `mne-1.4.2/mne/channels/data/layouts/Neuromag_122.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/Vectorview-all.lout` & `mne-1.4.2/mne/channels/data/layouts/Vectorview-all.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/Vectorview-grad.lout` & `mne-1.4.2/mne/channels/data/layouts/Vectorview-grad.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/Vectorview-grad_norm.lout` & `mne-1.4.2/mne/channels/data/layouts/Vectorview-grad_norm.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/Vectorview-mag.lout` & `mne-1.4.2/mne/channels/data/layouts/Vectorview-mag.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/biosemi.lay` & `mne-1.4.2/mne/channels/data/layouts/biosemi.lay`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/layouts/magnesWH3600.lout` & `mne-1.4.2/mne/channels/data/layouts/magnesWH3600.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/EGI_256.csd` & `mne-1.4.2/mne/channels/data/montages/EGI_256.csd`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-128.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-128.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-129.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-129.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-256.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-256.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-257.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-257.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-32.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-32.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-64_1.0.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-64_1.0.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/GSN-HydroCel-65_1.0.sfp` & `mne-1.4.2/mne/channels/data/montages/GSN-HydroCel-65_1.0.sfp`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/artinis-brite23.elc` & `mne-1.4.2/mne/channels/data/montages/artinis-brite23.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/biosemi128.txt` & `mne-1.4.2/mne/channels/data/montages/biosemi128.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/biosemi160.txt` & `mne-1.4.2/mne/channels/data/montages/biosemi160.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/biosemi256.txt` & `mne-1.4.2/mne/channels/data/montages/biosemi256.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/biosemi64.txt` & `mne-1.4.2/mne/channels/data/montages/biosemi64.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/brainproducts-RNP-BA-128.txt` & `mne-1.4.2/mne/channels/data/montages/brainproducts-RNP-BA-128.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/easycap-M1.txt` & `mne-1.4.2/mne/channels/data/montages/easycap-M1.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/easycap-M10.txt` & `mne-1.4.2/mne/channels/data/montages/easycap-M10.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/mgh60.elc` & `mne-1.4.2/mne/channels/data/montages/mgh60.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/mgh70.elc` & `mne-1.4.2/mne/channels/data/montages/mgh70.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_1005.elc` & `mne-1.4.2/mne/channels/data/montages/standard_1005.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_1020.elc` & `mne-1.4.2/mne/channels/data/montages/standard_1020.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_alphabetic.elc` & `mne-1.4.2/mne/channels/data/montages/standard_alphabetic.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_postfixed.elc` & `mne-1.4.2/mne/channels/data/montages/standard_postfixed.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_prefixed.elc` & `mne-1.4.2/mne/channels/data/montages/standard_prefixed.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/montages/standard_primed.elc` & `mne-1.4.2/mne/channels/data/montages/standard_primed.elc`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-157_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-157_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-208_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-208_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-NYU-2019_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-NYU-2019_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-1_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-1_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-2_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-2_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-3_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-3_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/KIT-UMD-4_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/KIT-UMD-4_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/biosemi32_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/biosemi32_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/biosemi64_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/biosemi64_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/bti148_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/bti148_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/bti248_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/bti248_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/bti248grad_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/bti248grad_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/ctf151_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/ctf151_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/ctf275_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/ctf275_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/ctf64_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/ctf64_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycap128ch-avg_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycap128ch-avg_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycap32ch-avg_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycap32ch-avg_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycap64ch-avg_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycap64ch-avg_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycapM11_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycapM11_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycapM14_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycapM14_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycapM15_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycapM15_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/easycapM1_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/easycapM1_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/ecog256_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/ecog256_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/ecog256bipolar_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/ecog256bipolar_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/eeg1010_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/eeg1010_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/elec1005_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/elec1005_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/elec1010_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/elec1010_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/elec1020_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/elec1020_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/itab153_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/itab153_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/itab28_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/itab28_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/language29ch-avg_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/language29ch-avg_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/mpi_59_channels_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/mpi_59_channels_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/neuromag122cmb_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/neuromag122cmb_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/neuromag306cmb_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/neuromag306cmb_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/neuromag306mag_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/neuromag306mag_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/neuromag306planar_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/neuromag306planar_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/yokogawa160_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/yokogawa160_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/data/neighbors/yokogawa440_neighb.mat` & `mne-1.4.2/mne/channels/data/neighbors/yokogawa440_neighb.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/interpolation.py` & `mne-1.4.2/mne/channels/interpolation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/layout.py` & `mne-1.4.2/mne/channels/layout.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/montage.py` & `mne-1.4.2/mne/channels/montage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/tests/test_channels.py` & `mne-1.4.2/mne/channels/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/tests/test_interpolation.py` & `mne-1.4.2/mne/channels/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/tests/test_layout.py` & `mne-1.4.2/mne/channels/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/tests/test_montage.py` & `mne-1.4.2/mne/channels/tests/test_montage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/channels/tests/test_standard_montage.py` & `mne-1.4.2/mne/channels/tests/test_standard_montage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/chpi.py` & `mne-1.4.2/mne/chpi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_anonymize.py` & `mne-1.4.2/mne/commands/mne_anonymize.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_browse_raw.py` & `mne-1.4.2/mne/commands/mne_browse_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_bti2fiff.py` & `mne-1.4.2/mne/commands/mne_bti2fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_clean_eog_ecg.py` & `mne-1.4.2/mne/commands/mne_clean_eog_ecg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_compare_fiff.py` & `mne-1.4.2/mne/commands/mne_compare_fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_compute_proj_ecg.py` & `mne-1.4.2/mne/commands/mne_compute_proj_ecg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_compute_proj_eog.py` & `mne-1.4.2/mne/commands/mne_compute_proj_eog.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_coreg.py` & `mne-1.4.2/mne/commands/mne_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_flash_bem.py` & `mne-1.4.2/mne/commands/mne_flash_bem.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_freeview_bem_surfaces.py` & `mne-1.4.2/mne/commands/mne_freeview_bem_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_kit2fiff.py` & `mne-1.4.2/mne/commands/mne_kit2fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_make_scalp_surfaces.py` & `mne-1.4.2/mne/commands/mne_make_scalp_surfaces.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_maxfilter.py` & `mne-1.4.2/mne/commands/mne_maxfilter.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_prepare_bem_model.py` & `mne-1.4.2/mne/commands/mne_prepare_bem_model.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_report.py` & `mne-1.4.2/mne/commands/mne_report.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_setup_forward_model.py` & `mne-1.4.2/mne/commands/mne_setup_forward_model.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_setup_source_space.py` & `mne-1.4.2/mne/commands/mne_setup_source_space.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_show_fiff.py` & `mne-1.4.2/mne/commands/mne_show_fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_show_info.py` & `mne-1.4.2/mne/commands/mne_show_info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_surf2bem.py` & `mne-1.4.2/mne/commands/mne_surf2bem.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_sys_info.py` & `mne-1.4.2/mne/commands/mne_sys_info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/mne_watershed_bem.py` & `mne-1.4.2/mne/commands/mne_watershed_bem.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/tests/test_commands.py` & `mne-1.4.2/mne/commands/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/commands/utils.py` & `mne-1.4.2/mne/commands/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/conftest.py` & `mne-1.4.2/mne/conftest.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/coreg.py` & `mne-1.4.2/mne/coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/cov.py` & `mne-1.4.2/mne/cov.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/cuda.py` & `mne-1.4.2/mne/cuda.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/FreeSurferColorLUT.txt` & `mne-1.4.2/mne/data/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/coil_def.dat` & `mne-1.4.2/mne/data/coil_def.dat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/coil_def_Elekta.dat` & `mne-1.4.2/mne/data/coil_def_Elekta.dat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/eegbci_checksums.txt` & `mne-1.4.2/mne/data/eegbci_checksums.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/extinction_coef.mat` & `mne-1.4.2/mne/data/extinction_coef.mat`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/fsaverage/fsaverage-head.fif` & `mne-1.4.2/mne/data/fsaverage/fsaverage-head.fif`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/fsaverage/fsaverage-inner_skull-bem.fif` & `mne-1.4.2/mne/data/fsaverage/fsaverage-inner_skull-bem.fif`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/122m.fif.gz` & `mne-1.4.2/mne/data/helmets/122m.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/306m.fif.gz` & `mne-1.4.2/mne/data/helmets/306m.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/306m_rt.fif.gz` & `mne-1.4.2/mne/data/helmets/306m_rt.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/BabySQUID.fif.gz` & `mne-1.4.2/mne/data/helmets/BabySQUID.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/CTF_275.fif.gz` & `mne-1.4.2/mne/data/helmets/CTF_275.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/KIT.fif.gz` & `mne-1.4.2/mne/data/helmets/KIT.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/Magnes_2500wh.fif.gz` & `mne-1.4.2/mne/data/helmets/Magnes_2500wh.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/helmets/Magnes_3600wh.fif.gz` & `mne-1.4.2/mne/data/helmets/Magnes_3600wh.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/icos.fif.gz` & `mne-1.4.2/mne/data/icos.fif.gz`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/image/custom_layout.lout` & `mne-1.4.2/mne/data/image/custom_layout.lout`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/image/mni_brain.gif` & `mne-1.4.2/mne/data/image/mni_brain.gif`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/data/mne_analyze.sel` & `mne-1.4.2/mne/data/mne_analyze.sel`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/__init__.py` & `mne-1.4.2/mne/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_fake/_fake.py` & `mne-1.4.2/mne/datasets/_fake/_fake.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_fetch.py` & `mne-1.4.2/mne/datasets/_fetch.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_fsaverage/base.py` & `mne-1.4.2/mne/datasets/_fsaverage/base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_fsaverage/root.txt` & `mne-1.4.2/mne/datasets/_fsaverage/root.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS1-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS1-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS10-5Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS10-5Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS12-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS12-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS15-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS15-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS18-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS18-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS2-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS2-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS2-0Weeks3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS2-0Weeks3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS2-0Years3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS2-0Years3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS3-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS3-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS4-5Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS4-5Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS6-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS6-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS7-5Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS7-5Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/ANTS9-0Months3T.txt` & `mne-1.4.2/mne/datasets/_infant/ANTS9-0Months3T.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_infant/base.py` & `mne-1.4.2/mne/datasets/_infant/base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/_phantom/base.py` & `mne-1.4.2/mne/datasets/_phantom/base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/brainstorm/bst_auditory.py` & `mne-1.4.2/mne/datasets/brainstorm/bst_auditory.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/brainstorm/bst_phantom_ctf.py` & `mne-1.4.2/mne/datasets/brainstorm/bst_phantom_ctf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/brainstorm/bst_phantom_elekta.py` & `mne-1.4.2/mne/datasets/brainstorm/bst_phantom_elekta.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/brainstorm/bst_raw.py` & `mne-1.4.2/mne/datasets/brainstorm/bst_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/brainstorm/bst_resting.py` & `mne-1.4.2/mne/datasets/brainstorm/bst_resting.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/config.py` & `mne-1.4.2/mne/datasets/config.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/eegbci/eegbci.py` & `mne-1.4.2/mne/datasets/eegbci/eegbci.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/epilepsy_ecog/_data.py` & `mne-1.4.2/mne/datasets/epilepsy_ecog/_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/erp_core/erp_core.py` & `mne-1.4.2/mne/datasets/erp_core/erp_core.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/eyelink/eyelink.py` & `mne-1.4.2/mne/datasets/eyelink/eyelink.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/fieldtrip_cmc/fieldtrip_cmc.py` & `mne-1.4.2/mne/datasets/fieldtrip_cmc/fieldtrip_cmc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/fnirs_motor/fnirs_motor.py` & `mne-1.4.2/mne/datasets/fnirs_motor/fnirs_motor.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/hf_sef/hf_sef.py` & `mne-1.4.2/mne/datasets/hf_sef/hf_sef.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/kiloword/kiloword.py` & `mne-1.4.2/mne/datasets/kiloword/kiloword.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/limo/limo.py` & `mne-1.4.2/mne/datasets/limo/limo.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/misc/_misc.py` & `mne-1.4.2/mne/datasets/misc/_misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/mtrf/mtrf.py` & `mne-1.4.2/mne/datasets/mtrf/mtrf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/multimodal/multimodal.py` & `mne-1.4.2/mne/datasets/multimodal/multimodal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/opm/opm.py` & `mne-1.4.2/mne/datasets/opm/opm.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/phantom_4dbti/phantom_4dbti.py` & `mne-1.4.2/mne/datasets/phantom_4dbti/phantom_4dbti.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/refmeg_noise/refmeg_noise.py` & `mne-1.4.2/mne/datasets/refmeg_noise/refmeg_noise.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sample/sample.py` & `mne-1.4.2/mne/datasets/sample/sample.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/SHA1SUMS` & `mne-1.4.2/mne/datasets/sleep_physionet/SHA1SUMS`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/_utils.py` & `mne-1.4.2/mne/datasets/sleep_physionet/_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/age.py` & `mne-1.4.2/mne/datasets/sleep_physionet/age.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/age_records.csv` & `mne-1.4.2/mne/datasets/sleep_physionet/age_records.csv`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/temazepam.py` & `mne-1.4.2/mne/datasets/sleep_physionet/temazepam.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/temazepam_records.csv` & `mne-1.4.2/mne/datasets/sleep_physionet/temazepam_records.csv`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/sleep_physionet/tests/test_physionet.py` & `mne-1.4.2/mne/datasets/sleep_physionet/tests/test_physionet.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/somato/somato.py` & `mne-1.4.2/mne/datasets/somato/somato.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/spm_face/spm_data.py` & `mne-1.4.2/mne/datasets/spm_face/spm_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/ssvep/ssvep.py` & `mne-1.4.2/mne/datasets/ssvep/ssvep.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/testing/_testing.py` & `mne-1.4.2/mne/datasets/testing/_testing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/tests/test_datasets.py` & `mne-1.4.2/mne/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/ucl_opm_auditory/ucl_opm_auditory.py` & `mne-1.4.2/mne/datasets/ucl_opm_auditory/ucl_opm_auditory.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/utils.py` & `mne-1.4.2/mne/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/datasets/visual_92_categories/visual_92_categories.py` & `mne-1.4.2/mne/datasets/visual_92_categories/visual_92_categories.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/__init__.py` & `mne-1.4.2/mne/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/base.py` & `mne-1.4.2/mne/decoding/base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/csp.py` & `mne-1.4.2/mne/decoding/csp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/ems.py` & `mne-1.4.2/mne/decoding/ems.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/mixin.py` & `mne-1.4.2/mne/decoding/mixin.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/receptive_field.py` & `mne-1.4.2/mne/decoding/receptive_field.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/search_light.py` & `mne-1.4.2/mne/decoding/search_light.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/ssd.py` & `mne-1.4.2/mne/decoding/ssd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_base.py` & `mne-1.4.2/mne/decoding/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_csp.py` & `mne-1.4.2/mne/decoding/tests/test_csp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_ems.py` & `mne-1.4.2/mne/decoding/tests/test_ems.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_receptive_field.py` & `mne-1.4.2/mne/decoding/tests/test_receptive_field.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_search_light.py` & `mne-1.4.2/mne/decoding/tests/test_search_light.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_ssd.py` & `mne-1.4.2/mne/decoding/tests/test_ssd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_time_frequency.py` & `mne-1.4.2/mne/decoding/tests/test_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/tests/test_transformer.py` & `mne-1.4.2/mne/decoding/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/time_delaying_ridge.py` & `mne-1.4.2/mne/decoding/time_delaying_ridge.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/time_frequency.py` & `mne-1.4.2/mne/decoding/time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/decoding/transformer.py` & `mne-1.4.2/mne/decoding/transformer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/defaults.py` & `mne-1.4.2/mne/defaults.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/dipole.py` & `mne-1.4.2/mne/dipole.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/epochs.py` & `mne-1.4.2/mne/epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/event.py` & `mne-1.4.2/mne/event.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/evoked.py` & `mne-1.4.2/mne/evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/export/_edf.py` & `mne-1.4.2/mne/export/_edf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/export/_eeglab.py` & `mne-1.4.2/mne/export/_eeglab.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/export/_egimff.py` & `mne-1.4.2/mne/export/_egimff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/export/_export.py` & `mne-1.4.2/mne/export/_export.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/export/tests/test_export.py` & `mne-1.4.2/mne/export/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/filter.py` & `mne-1.4.2/mne/filter.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/fixes.py` & `mne-1.4.2/mne/fixes.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/__init__.py` & `mne-1.4.2/mne/forward/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/_compute_forward.py` & `mne-1.4.2/mne/forward/_compute_forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/_field_interpolation.py` & `mne-1.4.2/mne/forward/_field_interpolation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/_lead_dots.py` & `mne-1.4.2/mne/forward/_lead_dots.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/_make_forward.py` & `mne-1.4.2/mne/forward/_make_forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/forward.py` & `mne-1.4.2/mne/forward/forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/tests/test_field_interpolation.py` & `mne-1.4.2/mne/forward/tests/test_field_interpolation.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/tests/test_forward.py` & `mne-1.4.2/mne/forward/tests/test_forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/forward/tests/test_make_forward.py` & `mne-1.4.2/mne/forward/tests/test_make_forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/__init__.py` & `mne-1.4.2/mne/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/_core.py` & `mne-1.4.2/mne/gui/_core.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/_coreg.py` & `mne-1.4.2/mne/gui/_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/_ieeg_locate.py` & `mne-1.4.2/mne/gui/_ieeg_locate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/tests/test_core.py` & `mne-1.4.2/mne/gui/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/tests/test_coreg.py` & `mne-1.4.2/mne/gui/tests/test_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/tests/test_gui_api.py` & `mne-1.4.2/mne/gui/tests/test_gui_api.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/gui/tests/test_ieeg_locate.py` & `mne-1.4.2/mne/gui/tests/test_ieeg_locate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html/d3.v3.min.js` & `mne-1.4.2/mne/html/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html/mpld3.v0.2.min.js` & `mne-1.4.2/mne/html/mpld3.v0.2.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/header.html.jinja` & `mne-1.4.2/mne/html_templates/report/header.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/html.html.jinja` & `mne-1.4.2/mne/html_templates/report/html.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/image.html.jinja` & `mne-1.4.2/mne/html_templates/report/image.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/section.html.jinja` & `mne-1.4.2/mne/html_templates/report/section.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/slider.html.jinja` & `mne-1.4.2/mne/html_templates/report/slider.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/report/toc.html.jinja` & `mne-1.4.2/mne/html_templates/report/toc.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/repr/epochs.html.jinja` & `mne-1.4.2/mne/html_templates/repr/epochs.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/repr/evoked.html.jinja` & `mne-1.4.2/mne/html_templates/repr/evoked.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/repr/ica.html.jinja` & `mne-1.4.2/mne/html_templates/repr/ica.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/repr/info.html.jinja` & `mne-1.4.2/mne/html_templates/repr/info.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/html_templates/repr/spectrum.html.jinja` & `mne-1.4.2/mne/html_templates/repr/spectrum.html.jinja`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/dark/actions/scale.svg` & `mne-1.4.2/mne/icons/dark/actions/scale.svg`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/dark/actions/visibility_off.svg` & `mne-1.4.2/mne/icons/dark/actions/visibility_off.svg`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/light/actions/scale.svg` & `mne-1.4.2/mne/icons/light/actions/scale.svg`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/light/actions/visibility_off.svg` & `mne-1.4.2/mne/icons/light/actions/visibility_off.svg`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/mne_bigsur_icon.png` & `mne-1.4.2/mne/icons/mne_bigsur_icon.png`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/mne_default_icon.png` & `mne-1.4.2/mne/icons/mne_default_icon.png`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/mne_icon-cropped.png` & `mne-1.4.2/mne/icons/mne_icon-cropped.png`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/mne_icon.png` & `mne-1.4.2/mne/icons/mne_icon.png`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/icons/mne_splash.png` & `mne-1.4.2/mne/icons/mne_splash.png`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/_gamma_map.py` & `mne-1.4.2/mne/inverse_sparse/_gamma_map.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/mxne_debiasing.py` & `mne-1.4.2/mne/inverse_sparse/mxne_debiasing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/mxne_inverse.py` & `mne-1.4.2/mne/inverse_sparse/mxne_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/mxne_optim.py` & `mne-1.4.2/mne/inverse_sparse/mxne_optim.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/tests/test_gamma_map.py` & `mne-1.4.2/mne/inverse_sparse/tests/test_gamma_map.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/tests/test_mxne_debiasing.py` & `mne-1.4.2/mne/inverse_sparse/tests/test_mxne_debiasing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/tests/test_mxne_inverse.py` & `mne-1.4.2/mne/inverse_sparse/tests/test_mxne_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/inverse_sparse/tests/test_mxne_optim.py` & `mne-1.4.2/mne/inverse_sparse/tests/test_mxne_optim.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/__init__.py` & `mne-1.4.2/mne/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/_digitization.py` & `mne-1.4.2/mne/io/_digitization.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/_read_raw.py` & `mne-1.4.2/mne/io/_read_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/array/array.py` & `mne-1.4.2/mne/io/array/array.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/array/tests/test_array.py` & `mne-1.4.2/mne/io/array/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/artemis123/artemis123.py` & `mne-1.4.2/mne/io/artemis123/artemis123.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/artemis123/resources/Artemis123_ChannelMap.csv` & `mne-1.4.2/mne/io/artemis123/resources/Artemis123_ChannelMap.csv`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/artemis123/resources/Artemis123_mneLoc.csv` & `mne-1.4.2/mne/io/artemis123/resources/Artemis123_mneLoc.csv`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/artemis123/tests/test_artemis123.py` & `mne-1.4.2/mne/io/artemis123/tests/test_artemis123.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/artemis123/utils.py` & `mne-1.4.2/mne/io/artemis123/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/base.py` & `mne-1.4.2/mne/io/base.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/besa/besa.py` & `mne-1.4.2/mne/io/besa/besa.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/besa/tests/test_besa.py` & `mne-1.4.2/mne/io/besa/tests/test_besa.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/boxy/boxy.py` & `mne-1.4.2/mne/io/boxy/boxy.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/boxy/tests/test_boxy.py` & `mne-1.4.2/mne/io/boxy/tests/test_boxy.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/brainvision/brainvision.py` & `mne-1.4.2/mne/io/brainvision/brainvision.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/brainvision/tests/test_brainvision.py` & `mne-1.4.2/mne/io/brainvision/tests/test_brainvision.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/bti/bti.py` & `mne-1.4.2/mne/io/bti/bti.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/bti/constants.py` & `mne-1.4.2/mne/io/bti/constants.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/bti/read.py` & `mne-1.4.2/mne/io/bti/read.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/bti/tests/test_bti.py` & `mne-1.4.2/mne/io/bti/tests/test_bti.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/cnt/_utils.py` & `mne-1.4.2/mne/io/cnt/_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/cnt/cnt.py` & `mne-1.4.2/mne/io/cnt/cnt.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/cnt/tests/test_cnt.py` & `mne-1.4.2/mne/io/cnt/tests/test_cnt.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/compensator.py` & `mne-1.4.2/mne/io/compensator.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/constants.py` & `mne-1.4.2/mne/io/constants.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/constants.py` & `mne-1.4.2/mne/io/ctf/constants.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/ctf.py` & `mne-1.4.2/mne/io/ctf/ctf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/eeg.py` & `mne-1.4.2/mne/io/ctf/eeg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/hc.py` & `mne-1.4.2/mne/io/ctf/hc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/info.py` & `mne-1.4.2/mne/io/ctf/info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/markers.py` & `mne-1.4.2/mne/io/ctf/markers.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/res4.py` & `mne-1.4.2/mne/io/ctf/res4.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/tests/test_ctf.py` & `mne-1.4.2/mne/io/ctf/tests/test_ctf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf/trans.py` & `mne-1.4.2/mne/io/ctf/trans.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/ctf_comp.py` & `mne-1.4.2/mne/io/ctf_comp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/curry/curry.py` & `mne-1.4.2/mne/io/curry/curry.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/curry/tests/test_curry.py` & `mne-1.4.2/mne/io/curry/tests/test_curry.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/diff.py` & `mne-1.4.2/mne/io/diff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/edf/edf.py` & `mne-1.4.2/mne/io/edf/edf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/edf/tests/test_edf.py` & `mne-1.4.2/mne/io/edf/tests/test_edf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/edf/tests/test_gdf.py` & `mne-1.4.2/mne/io/edf/tests/test_gdf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eeglab/_eeglab.py` & `mne-1.4.2/mne/io/eeglab/_eeglab.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eeglab/eeglab.py` & `mne-1.4.2/mne/io/eeglab/eeglab.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eeglab/tests/test_eeglab.py` & `mne-1.4.2/mne/io/eeglab/tests/test_eeglab.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/egi/egi.py` & `mne-1.4.2/mne/io/egi/egi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/egi/egimff.py` & `mne-1.4.2/mne/io/egi/egimff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/egi/events.py` & `mne-1.4.2/mne/io/egi/events.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/egi/general.py` & `mne-1.4.2/mne/io/egi/general.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/egi/tests/test_egi.py` & `mne-1.4.2/mne/io/egi/tests/test_egi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eximia/eximia.py` & `mne-1.4.2/mne/io/eximia/eximia.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eximia/tests/test_eximia.py` & `mne-1.4.2/mne/io/eximia/tests/test_eximia.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eyelink/eyelink.py` & `mne-1.4.2/mne/io/eyelink/eyelink.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/eyelink/tests/test_eyelink.py` & `mne-1.4.2/mne/io/eyelink/tests/test_eyelink.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fieldtrip/fieldtrip.py` & `mne-1.4.2/mne/io/fieldtrip/fieldtrip.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fieldtrip/tests/helpers.py` & `mne-1.4.2/mne/io/fieldtrip/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fieldtrip/tests/test_fieldtrip.py` & `mne-1.4.2/mne/io/fieldtrip/tests/test_fieldtrip.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fieldtrip/utils.py` & `mne-1.4.2/mne/io/fieldtrip/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fiff/raw.py` & `mne-1.4.2/mne/io/fiff/raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fiff/tests/test_raw_fiff.py` & `mne-1.4.2/mne/io/fiff/tests/test_raw_fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fil/fil.py` & `mne-1.4.2/mne/io/fil/fil.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fil/sensors.py` & `mne-1.4.2/mne/io/fil/sensors.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/fil/tests/test_fil.py` & `mne-1.4.2/mne/io/fil/tests/test_fil.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/hitachi/hitachi.py` & `mne-1.4.2/mne/io/hitachi/hitachi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/hitachi/tests/test_hitachi.py` & `mne-1.4.2/mne/io/hitachi/tests/test_hitachi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/kit/constants.py` & `mne-1.4.2/mne/io/kit/constants.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/kit/coreg.py` & `mne-1.4.2/mne/io/kit/coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/kit/kit.py` & `mne-1.4.2/mne/io/kit/kit.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/kit/tests/test_coreg.py` & `mne-1.4.2/mne/io/kit/tests/test_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/kit/tests/test_kit.py` & `mne-1.4.2/mne/io/kit/tests/test_kit.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/matrix.py` & `mne-1.4.2/mne/io/matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/meas_info.py` & `mne-1.4.2/mne/io/meas_info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nedf/nedf.py` & `mne-1.4.2/mne/io/nedf/nedf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nedf/tests/test_nedf.py` & `mne-1.4.2/mne/io/nedf/tests/test_nedf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nicolet/nicolet.py` & `mne-1.4.2/mne/io/nicolet/nicolet.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nicolet/tests/test_nicolet.py` & `mne-1.4.2/mne/io/nicolet/tests/test_nicolet.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nihon/nihon.py` & `mne-1.4.2/mne/io/nihon/nihon.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nihon/tests/test_nihon.py` & `mne-1.4.2/mne/io/nihon/tests/test_nihon.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nirx/_localized_abbr.py` & `mne-1.4.2/mne/io/nirx/_localized_abbr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nirx/nirx.py` & `mne-1.4.2/mne/io/nirx/nirx.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/nirx/tests/test_nirx.py` & `mne-1.4.2/mne/io/nirx/tests/test_nirx.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/open.py` & `mne-1.4.2/mne/io/open.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/persyst/persyst.py` & `mne-1.4.2/mne/io/persyst/persyst.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/persyst/tests/test_persyst.py` & `mne-1.4.2/mne/io/persyst/tests/test_persyst.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/pick.py` & `mne-1.4.2/mne/io/pick.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/proc_history.py` & `mne-1.4.2/mne/io/proc_history.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/proj.py` & `mne-1.4.2/mne/io/proj.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/reference.py` & `mne-1.4.2/mne/io/reference.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/snirf/_snirf.py` & `mne-1.4.2/mne/io/snirf/_snirf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/snirf/tests/test_snirf.py` & `mne-1.4.2/mne/io/snirf/tests/test_snirf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tag.py` & `mne-1.4.2/mne/io/tag.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_apply_function.py` & `mne-1.4.2/mne/io/tests/test_apply_function.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_compensator.py` & `mne-1.4.2/mne/io/tests/test_compensator.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_constants.py` & `mne-1.4.2/mne/io/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_meas_info.py` & `mne-1.4.2/mne/io/tests/test_meas_info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_pick.py` & `mne-1.4.2/mne/io/tests/test_pick.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_proc_history.py` & `mne-1.4.2/mne/io/tests/test_proc_history.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_raw.py` & `mne-1.4.2/mne/io/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_read_raw.py` & `mne-1.4.2/mne/io/tests/test_read_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_reference.py` & `mne-1.4.2/mne/io/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_show_fiff.py` & `mne-1.4.2/mne/io/tests/test_show_fiff.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_utils.py` & `mne-1.4.2/mne/io/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_what.py` & `mne-1.4.2/mne/io/tests/test_what.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tests/test_write.py` & `mne-1.4.2/mne/io/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/tree.py` & `mne-1.4.2/mne/io/tree.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/utils.py` & `mne-1.4.2/mne/io/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/what.py` & `mne-1.4.2/mne/io/what.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/io/write.py` & `mne-1.4.2/mne/io/write.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/label.py` & `mne-1.4.2/mne/label.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/__init__.py` & `mne-1.4.2/mne/minimum_norm/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/_eloreta.py` & `mne-1.4.2/mne/minimum_norm/_eloreta.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/inverse.py` & `mne-1.4.2/mne/minimum_norm/inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/resolution_matrix.py` & `mne-1.4.2/mne/minimum_norm/resolution_matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/spatial_resolution.py` & `mne-1.4.2/mne/minimum_norm/spatial_resolution.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/tests/test_inverse.py` & `mne-1.4.2/mne/minimum_norm/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/tests/test_resolution_matrix.py` & `mne-1.4.2/mne/minimum_norm/tests/test_resolution_matrix.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/tests/test_resolution_metrics.py` & `mne-1.4.2/mne/minimum_norm/tests/test_resolution_metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/tests/test_snr.py` & `mne-1.4.2/mne/minimum_norm/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/tests/test_time_frequency.py` & `mne-1.4.2/mne/minimum_norm/tests/test_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/minimum_norm/time_frequency.py` & `mne-1.4.2/mne/minimum_norm/time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/misc.py` & `mne-1.4.2/mne/misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/morph.py` & `mne-1.4.2/mne/morph.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/morph_map.py` & `mne-1.4.2/mne/morph_map.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/parallel.py` & `mne-1.4.2/mne/parallel.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/__init__.py` & `mne-1.4.2/mne/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/_csd.py` & `mne-1.4.2/mne/preprocessing/_csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/_css.py` & `mne-1.4.2/mne/preprocessing/_css.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/_fine_cal.py` & `mne-1.4.2/mne/preprocessing/_fine_cal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/_peak_finder.py` & `mne-1.4.2/mne/preprocessing/_peak_finder.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/_regress.py` & `mne-1.4.2/mne/preprocessing/_regress.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/annotate_amplitude.py` & `mne-1.4.2/mne/preprocessing/annotate_amplitude.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/annotate_nan.py` & `mne-1.4.2/mne/preprocessing/annotate_nan.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/artifact_detection.py` & `mne-1.4.2/mne/preprocessing/artifact_detection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/bads.py` & `mne-1.4.2/mne/preprocessing/bads.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ctps_.py` & `mne-1.4.2/mne/preprocessing/ctps_.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ecg.py` & `mne-1.4.2/mne/preprocessing/ecg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/eog.py` & `mne-1.4.2/mne/preprocessing/eog.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/eyetracking/eyetracking.py` & `mne-1.4.2/mne/preprocessing/eyetracking/eyetracking.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/hfc.py` & `mne-1.4.2/mne/preprocessing/hfc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ica.py` & `mne-1.4.2/mne/preprocessing/ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ieeg/_projection.py` & `mne-1.4.2/mne/preprocessing/ieeg/_projection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ieeg/_volume.py` & `mne-1.4.2/mne/preprocessing/ieeg/_volume.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ieeg/tests/test_projection.py` & `mne-1.4.2/mne/preprocessing/ieeg/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ieeg/tests/test_volume.py` & `mne-1.4.2/mne/preprocessing/ieeg/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/infomax_.py` & `mne-1.4.2/mne/preprocessing/infomax_.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/interpolate.py` & `mne-1.4.2/mne/preprocessing/interpolate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/maxfilter.py` & `mne-1.4.2/mne/preprocessing/maxfilter.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/maxwell.py` & `mne-1.4.2/mne/preprocessing/maxwell.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/__init__.py` & `mne-1.4.2/mne/preprocessing/nirs/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/_beer_lambert_law.py` & `mne-1.4.2/mne/preprocessing/nirs/_beer_lambert_law.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/_optical_density.py` & `mne-1.4.2/mne/preprocessing/nirs/_optical_density.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/_scalp_coupling_index.py` & `mne-1.4.2/mne/preprocessing/nirs/_scalp_coupling_index.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/_tddr.py` & `mne-1.4.2/mne/preprocessing/nirs/_tddr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/nirs.py` & `mne-1.4.2/mne/preprocessing/nirs/nirs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/tests/test_beer_lambert_law.py` & `mne-1.4.2/mne/preprocessing/nirs/tests/test_beer_lambert_law.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/tests/test_nirs.py` & `mne-1.4.2/mne/preprocessing/nirs/tests/test_nirs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/tests/test_optical_density.py` & `mne-1.4.2/mne/preprocessing/nirs/tests/test_optical_density.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/tests/test_scalp_coupling_index.py` & `mne-1.4.2/mne/preprocessing/nirs/tests/test_scalp_coupling_index.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/nirs/tests/test_temporal_derivative_distribution_repair.py` & `mne-1.4.2/mne/preprocessing/nirs/tests/test_temporal_derivative_distribution_repair.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/otp.py` & `mne-1.4.2/mne/preprocessing/otp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/realign.py` & `mne-1.4.2/mne/preprocessing/realign.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/ssp.py` & `mne-1.4.2/mne/preprocessing/ssp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/stim.py` & `mne-1.4.2/mne/preprocessing/stim.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_annotate_amplitude.py` & `mne-1.4.2/mne/preprocessing/tests/test_annotate_amplitude.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_annotate_nan.py` & `mne-1.4.2/mne/preprocessing/tests/test_annotate_nan.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_artifact_detection.py` & `mne-1.4.2/mne/preprocessing/tests/test_artifact_detection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_csd.py` & `mne-1.4.2/mne/preprocessing/tests/test_csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_css.py` & `mne-1.4.2/mne/preprocessing/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_ctps.py` & `mne-1.4.2/mne/preprocessing/tests/test_ctps.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_ecg.py` & `mne-1.4.2/mne/preprocessing/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_eeglab_infomax.py` & `mne-1.4.2/mne/preprocessing/tests/test_eeglab_infomax.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_eog.py` & `mne-1.4.2/mne/preprocessing/tests/test_eog.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_fine_cal.py` & `mne-1.4.2/mne/preprocessing/tests/test_fine_cal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_hfc.py` & `mne-1.4.2/mne/preprocessing/tests/test_hfc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_ica.py` & `mne-1.4.2/mne/preprocessing/tests/test_ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_infomax.py` & `mne-1.4.2/mne/preprocessing/tests/test_infomax.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_interpolate.py` & `mne-1.4.2/mne/preprocessing/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_maxwell.py` & `mne-1.4.2/mne/preprocessing/tests/test_maxwell.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_otp.py` & `mne-1.4.2/mne/preprocessing/tests/test_otp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_peak_finder.py` & `mne-1.4.2/mne/preprocessing/tests/test_peak_finder.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_realign.py` & `mne-1.4.2/mne/preprocessing/tests/test_realign.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_regress.py` & `mne-1.4.2/mne/preprocessing/tests/test_regress.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_ssp.py` & `mne-1.4.2/mne/preprocessing/tests/test_ssp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_stim.py` & `mne-1.4.2/mne/preprocessing/tests/test_stim.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/tests/test_xdawn.py` & `mne-1.4.2/mne/preprocessing/tests/test_xdawn.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/preprocessing/xdawn.py` & `mne-1.4.2/mne/preprocessing/xdawn.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/proj.py` & `mne-1.4.2/mne/proj.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/rank.py` & `mne-1.4.2/mne/rank.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-icons/bootstrap-icons.mne.min.css` & `mne-1.4.2/mne/report/js_and_css/bootstrap-icons/bootstrap-icons.mne.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-icons/gen_css_for_mne.py` & `mne-1.4.2/mne/report/js_and_css/bootstrap-icons/gen_css_for_mne.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table-copy-rows.min.js` & `mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table-copy-rows.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table-export.min.js` & `mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table-export.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.css` & `mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.js` & `mne-1.4.2/mne/report/js_and_css/bootstrap-table/bootstrap-table.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap-table/tableExport.min.js` & `mne-1.4.2/mne/report/js_and_css/bootstrap-table/tableExport.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap.bundle.min.js` & `mne-1.4.2/mne/report/js_and_css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/bootstrap.min.css` & `mne-1.4.2/mne/report/js_and_css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/highlightjs/atom-one-dark-reasonable.min.css` & `mne-1.4.2/mne/report/js_and_css/highlightjs/atom-one-dark-reasonable.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/highlightjs/atom-one-light.min.css` & `mne-1.4.2/mne/report/js_and_css/highlightjs/atom-one-light.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/highlightjs/default.min.css` & `mne-1.4.2/mne/report/js_and_css/highlightjs/default.min.css`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/highlightjs/highlight.min.js` & `mne-1.4.2/mne/report/js_and_css/highlightjs/highlight.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/jquery-3.6.0.min.js` & `mne-1.4.2/mne/report/js_and_css/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/js_and_css/report.js` & `mne-1.4.2/mne/report/js_and_css/report.js`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/report.py` & `mne-1.4.2/mne/report/report.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/report/tests/test_report.py` & `mne-1.4.2/mne/report/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/evoked.py` & `mne-1.4.2/mne/simulation/evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/metrics/metrics.py` & `mne-1.4.2/mne/simulation/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/metrics/tests/test_metrics.py` & `mne-1.4.2/mne/simulation/metrics/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/raw.py` & `mne-1.4.2/mne/simulation/raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/source.py` & `mne-1.4.2/mne/simulation/source.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/tests/test_evoked.py` & `mne-1.4.2/mne/simulation/tests/test_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/tests/test_metrics.py` & `mne-1.4.2/mne/simulation/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/tests/test_raw.py` & `mne-1.4.2/mne/simulation/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/simulation/tests/test_source.py` & `mne-1.4.2/mne/simulation/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/source_estimate.py` & `mne-1.4.2/mne/source_estimate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/source_space.py` & `mne-1.4.2/mne/source_space.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/__init__.py` & `mne-1.4.2/mne/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/_adjacency.py` & `mne-1.4.2/mne/stats/_adjacency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/cluster_level.py` & `mne-1.4.2/mne/stats/cluster_level.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/multi_comp.py` & `mne-1.4.2/mne/stats/multi_comp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/parametric.py` & `mne-1.4.2/mne/stats/parametric.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/permutations.py` & `mne-1.4.2/mne/stats/permutations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/regression.py` & `mne-1.4.2/mne/stats/regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_adjacency.py` & `mne-1.4.2/mne/stats/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_cluster_level.py` & `mne-1.4.2/mne/stats/tests/test_cluster_level.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_multi_comp.py` & `mne-1.4.2/mne/stats/tests/test_multi_comp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_parametric.py` & `mne-1.4.2/mne/stats/tests/test_parametric.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_permutations.py` & `mne-1.4.2/mne/stats/tests/test_permutations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/stats/tests/test_regression.py` & `mne-1.4.2/mne/stats/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/surface.py` & `mne-1.4.2/mne/surface.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_annotations.py` & `mne-1.4.2/mne/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_bem.py` & `mne-1.4.2/mne/tests/test_bem.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_chpi.py` & `mne-1.4.2/mne/tests/test_chpi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_coreg.py` & `mne-1.4.2/mne/tests/test_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_cov.py` & `mne-1.4.2/mne/tests/test_cov.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_defaults.py` & `mne-1.4.2/mne/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_dipole.py` & `mne-1.4.2/mne/tests/test_dipole.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_docstring_parameters.py` & `mne-1.4.2/mne/tests/test_docstring_parameters.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_epochs.py` & `mne-1.4.2/mne/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_event.py` & `mne-1.4.2/mne/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_evoked.py` & `mne-1.4.2/mne/tests/test_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_filter.py` & `mne-1.4.2/mne/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_freesurfer.py` & `mne-1.4.2/mne/tests/test_freesurfer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_import_nesting.py` & `mne-1.4.2/mne/tests/test_import_nesting.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_label.py` & `mne-1.4.2/mne/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_line_endings.py` & `mne-1.4.2/mne/tests/test_line_endings.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_morph.py` & `mne-1.4.2/mne/tests/test_morph.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_morph_map.py` & `mne-1.4.2/mne/tests/test_morph_map.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_ola.py` & `mne-1.4.2/mne/tests/test_ola.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_parallel.py` & `mne-1.4.2/mne/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_proj.py` & `mne-1.4.2/mne/tests/test_proj.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_rank.py` & `mne-1.4.2/mne/tests/test_rank.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_read_vectorview_selection.py` & `mne-1.4.2/mne/tests/test_read_vectorview_selection.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_source_estimate.py` & `mne-1.4.2/mne/tests/test_source_estimate.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_source_space.py` & `mne-1.4.2/mne/tests/test_source_space.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_surface.py` & `mne-1.4.2/mne/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/tests/test_transforms.py` & `mne-1.4.2/mne/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/__init__.py` & `mne-1.4.2/mne/time_frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/_stft.py` & `mne-1.4.2/mne/time_frequency/_stft.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/_stockwell.py` & `mne-1.4.2/mne/time_frequency/_stockwell.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/ar.py` & `mne-1.4.2/mne/time_frequency/ar.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/csd.py` & `mne-1.4.2/mne/time_frequency/csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/multitaper.py` & `mne-1.4.2/mne/time_frequency/multitaper.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/psd.py` & `mne-1.4.2/mne/time_frequency/psd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/spectrum.py` & `mne-1.4.2/mne/time_frequency/spectrum.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_ar.py` & `mne-1.4.2/mne/time_frequency/tests/test_ar.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_csd.py` & `mne-1.4.2/mne/time_frequency/tests/test_csd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_multitaper.py` & `mne-1.4.2/mne/time_frequency/tests/test_multitaper.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_psd.py` & `mne-1.4.2/mne/time_frequency/tests/test_psd.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_spectrum.py` & `mne-1.4.2/mne/time_frequency/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_stft.py` & `mne-1.4.2/mne/time_frequency/tests/test_stft.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_stockwell.py` & `mne-1.4.2/mne/time_frequency/tests/test_stockwell.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tests/test_tfr.py` & `mne-1.4.2/mne/time_frequency/tests/test_tfr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/time_frequency/tfr.py` & `mne-1.4.2/mne/time_frequency/tfr.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/transforms.py` & `mne-1.4.2/mne/transforms.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/__init__.py` & `mne-1.4.2/mne/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/_bunch.py` & `mne-1.4.2/mne/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/_logging.py` & `mne-1.4.2/mne/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/_testing.py` & `mne-1.4.2/mne/utils/_testing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/check.py` & `mne-1.4.2/mne/utils/check.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/config.py` & `mne-1.4.2/mne/utils/config.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/dataframe.py` & `mne-1.4.2/mne/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/docs.py` & `mne-1.4.2/mne/utils/docs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/fetching.py` & `mne-1.4.2/mne/utils/fetching.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/linalg.py` & `mne-1.4.2/mne/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/misc.py` & `mne-1.4.2/mne/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/mixin.py` & `mne-1.4.2/mne/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/numerics.py` & `mne-1.4.2/mne/utils/numerics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/progressbar.py` & `mne-1.4.2/mne/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/spectrum.py` & `mne-1.4.2/mne/utils/spectrum.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_bunch.py` & `mne-1.4.2/mne/utils/tests/test_bunch.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_check.py` & `mne-1.4.2/mne/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_config.py` & `mne-1.4.2/mne/utils/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_docs.py` & `mne-1.4.2/mne/utils/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_linalg.py` & `mne-1.4.2/mne/utils/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_logging.py` & `mne-1.4.2/mne/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_misc.py` & `mne-1.4.2/mne/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_numerics.py` & `mne-1.4.2/mne/utils/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_progressbar.py` & `mne-1.4.2/mne/utils/tests/test_progressbar.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/utils/tests/test_testing.py` & `mne-1.4.2/mne/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_3d.py` & `mne-1.4.2/mne/viz/_3d.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_3d_overlay.py` & `mne-1.4.2/mne/viz/_3d_overlay.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/__init__.py` & `mne-1.4.2/mne/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/_brain.py` & `mne-1.4.2/mne/viz/_brain/_brain.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/_linkviewer.py` & `mne-1.4.2/mne/viz/_brain/_linkviewer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/_scraper.py` & `mne-1.4.2/mne/viz/_brain/_scraper.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/callback.py` & `mne-1.4.2/mne/viz/_brain/callback.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/colormap.py` & `mne-1.4.2/mne/viz/_brain/colormap.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/surface.py` & `mne-1.4.2/mne/viz/_brain/surface.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/tests/test_brain.py` & `mne-1.4.2/mne/viz/_brain/tests/test_brain.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/tests/test_notebook.py` & `mne-1.4.2/mne/viz/_brain/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_brain/view.py` & `mne-1.4.2/mne/viz/_brain/view.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_dipole.py` & `mne-1.4.2/mne/viz/_dipole.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_figure.py` & `mne-1.4.2/mne/viz/_figure.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_mpl_figure.py` & `mne-1.4.2/mne/viz/_mpl_figure.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_proj.py` & `mne-1.4.2/mne/viz/_proj.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/_scraper.py` & `mne-1.4.2/mne/viz/_scraper.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/_abstract.py` & `mne-1.4.2/mne/viz/backends/_abstract.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/_notebook.py` & `mne-1.4.2/mne/viz/backends/_notebook.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/_pyvista.py` & `mne-1.4.2/mne/viz/backends/_pyvista.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,19 @@
 
 
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import pyvista
     from pyvista import Plotter, PolyData, Line, close_all, UnstructuredGrid
     from pyvistaqt import BackgroundPlotter
-    from pyvista.plotting.plotting import _ALL_PLOTTERS
+
+    try:
+        from pyvista.plotting.plotter import _ALL_PLOTTERS
+    except Exception:  # PV < 0.40
+        from pyvista.plotting.plotting import _ALL_PLOTTERS
 
 from vtkmodules.vtkCommonCore import vtkCommand, vtkLookupTable, VTK_UNSIGNED_CHAR
 from vtkmodules.vtkCommonDataModel import VTK_VERTEX, vtkPiecewiseFunction
 from vtkmodules.vtkCommonTransforms import vtkTransform
 from vtkmodules.vtkFiltersCore import vtkCellDataToPointData, vtkGlyph3D
 from vtkmodules.vtkFiltersGeneral import (
     vtkTransformPolyDataFilter,
```

### Comparing `mne-1.4.1/mne/viz/backends/_qt.py` & `mne-1.4.2/mne/viz/backends/_qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,16 @@
         self.setText(value)
 
 
 class _Button(QPushButton, _AbstractButton, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, callback, icon=None):
         _AbstractButton.__init__(value=value, callback=callback)
         _Widget.__init__(self)
-        QPushButton.__init__(self)
+        with _disabled_init(_AbstractButton):
+            QPushButton.__init__(self)
         self.setText(value)
         self.released.connect(callback)
         if icon:
             self.setIcon(QIcon.fromTheme(icon))
 
     def _click(self):
         self.click()
@@ -284,15 +285,16 @@
 
 class _Slider(QSlider, _AbstractSlider, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, rng, callback, horizontal=True):
         _AbstractSlider.__init__(
             value=value, rng=rng, callback=callback, horizontal=horizontal
         )
         _Widget.__init__(self)
-        QSlider.__init__(self, Qt.Horizontal if horizontal else Qt.Vertical)
+        with _disabled_init(_AbstractSlider):
+            QSlider.__init__(self, Qt.Horizontal if horizontal else Qt.Vertical)
         self.setMinimum(rng[0])
         self.setMaximum(rng[1])
         self.setValue(value)
         self.valueChanged.connect(callback)
 
     def _set_value(self, value):
         self.setValue(value)
@@ -318,30 +320,32 @@
         return self.value()
 
 
 class _CheckBox(QCheckBox, _AbstractCheckBox, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, callback):
         _AbstractCheckBox.__init__(value=value, callback=callback)
         _Widget.__init__(self)
-        QCheckBox.__init__(self)
+        with _disabled_init(_AbstractCheckBox):
+            QCheckBox.__init__(self)
         self.setChecked(value)
         self.stateChanged.connect(lambda x: callback(bool(x)))
 
     def _set_checked(self, checked):
         self.setChecked(checked)
 
     def _get_checked(self):
         return self.checkState() != Qt.Unchecked
 
 
 class _SpinBox(QDoubleSpinBox, _AbstractSpinBox, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, rng, callback, step=None):
         _AbstractSpinBox.__init__(value=value, rng=rng, callback=callback, step=step)
         _Widget.__init__(self)
-        QDoubleSpinBox.__init__(self)
+        with _disabled_init(_AbstractSpinBox):
+            QDoubleSpinBox.__init__(self)
         self.setAlignment(Qt.AlignCenter)
         self.setMinimum(rng[0])
         self.setMaximum(rng[1])
         self.setKeyboardTracking(False)
         if step is None:
             self.setSingleStep((rng[1] - rng[0]) / 20.0)
         else:
@@ -356,15 +360,16 @@
         return self.value()
 
 
 class _ComboBox(QComboBox, _AbstractComboBox, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, items, callback):
         _AbstractComboBox.__init__(value=value, items=items, callback=callback)
         _Widget.__init__(self)
-        QComboBox.__init__(self)
+        with _disabled_init(_AbstractComboBox):
+            QComboBox.__init__(self)
         self.addItems(items)
         self.setCurrentText(value)
         self.currentTextChanged.connect(callback)
         self.setSizeAdjustPolicy(QComboBox.AdjustToContents)
 
     def _set_value(self, value):
         self.setCurrentText(value)
@@ -373,15 +378,16 @@
         return self.currentText()
 
 
 class _RadioButtons(QVBoxLayout, _AbstractRadioButtons, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, items, callback):
         _AbstractRadioButtons.__init__(value=value, items=items, callback=callback)
         _Widget.__init__(self)
-        QVBoxLayout.__init__(self)
+        with _disabled_init(_AbstractRadioButtons):
+            QVBoxLayout.__init__(self)
         self._button_group = QButtonGroup()
         self._button_group.setExclusive(True)
         for val in items:
             button = QRadioButton(val)
             if val == value:
                 button.setChecked(True)
             self._button_group.addButton(button)
@@ -451,15 +457,16 @@
         _Button.__init__(self, "", callback=fp_callback, icon=icon)
 
 
 class _PlayMenu(QVBoxLayout, _AbstractPlayMenu, _Widget, metaclass=_BaseWidget):
     def __init__(self, value, rng, callback):
         _AbstractPlayMenu.__init__(value=value, rng=rng, callback=callback)
         _Widget.__init__(self)
-        QVBoxLayout.__init__(self)
+        with _disabled_init(_AbstractPlayMenu):
+            QVBoxLayout.__init__(self)
         self._slider = QSlider(Qt.Horizontal)
         self._slider.setMinimum(rng[0])
         self._slider.setMaximum(rng[1])
         self._slider.setValue(value)
         self._slider.setTracking(False)
         self._slider.valueChanged.connect(callback)
         self._nav_hbox = QHBoxLayout()
@@ -536,15 +543,16 @@
             info_text=info_text,
             callback=callback,
             icon=icon,
             buttons=buttons,
             window=window,
         )
         _Widget.__init__(self)
-        QMessageBox.__init__(self, parent=window)
+        with _disabled_init(_AbstractPopup):
+            QMessageBox.__init__(self, parent=window)
         self.setWindowTitle(title)
         self.setText(text)
         # icon is one of _Dialog.supported_icon_names
         if icon is not None:
             self.setIcon(getattr(QMessageBox, icon.title()))
         if info_text:
             self.setInformativeText(info_text)
@@ -689,17 +697,30 @@
 # In theory we should be able to do this later (e.g., in _pyvista.py when
 # initializing), but at least on Qt6 this has to be done earlier. So let's do
 # it immediately upon instantiation of the QMainWindow class.
 # TODO: This should eventually allow us to handle
 # https://github.com/mne-tools/mne-python/issues/9182
 
 
+# This is necessary to make PySide6 happy -- something weird with the
+# __init__ calling causes the _AbstractXYZ class __init__ to be called twice
+@contextmanager
+def _disabled_init(klass):
+    orig = klass.__init__
+    klass.__init__ = lambda *args, **kwargs: None
+    try:
+        yield
+    finally:
+        klass.__init__ = orig
+
+
 class _MNEMainWindow(MainWindow):
     def __init__(self, parent=None, title=None, size=None):
-        MainWindow.__init__(self, parent=parent, title=title, size=size)
+        with _disabled_init(_Widget):
+            MainWindow.__init__(self, parent=parent, title=title, size=size)
         self.setAttribute(Qt.WA_ShowWithoutActivating, True)
         self.setAttribute(Qt.WA_DeleteOnClose, True)
 
 
 class _AppWindow(_AbstractAppWindow, _MNEMainWindow, _Widget, metaclass=_BaseWidget):
     def __init__(self, size=None, fullscreen=False):
         self._app = _init_mne_qtapp()
```

### Comparing `mne-1.4.1/mne/viz/backends/_utils.py` & `mne-1.4.2/mne/viz/backends/_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/renderer.py` & `mne-1.4.2/mne/viz/backends/renderer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/tests/_utils.py` & `mne-1.4.2/mne/viz/backends/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/tests/test_abstract.py` & `mne-1.4.2/mne/viz/backends/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/tests/test_renderer.py` & `mne-1.4.2/mne/viz/backends/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/backends/tests/test_utils.py` & `mne-1.4.2/mne/viz/backends/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/circle.py` & `mne-1.4.2/mne/viz/circle.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/conftest.py` & `mne-1.4.2/mne/viz/conftest.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/epochs.py` & `mne-1.4.2/mne/viz/epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/evoked.py` & `mne-1.4.2/mne/viz/evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/ica.py` & `mne-1.4.2/mne/viz/ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/misc.py` & `mne-1.4.2/mne/viz/misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/montage.py` & `mne-1.4.2/mne/viz/montage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/raw.py` & `mne-1.4.2/mne/viz/raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_3d.py` & `mne-1.4.2/mne/viz/tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_3d_mpl.py` & `mne-1.4.2/mne/viz/tests/test_3d_mpl.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_circle.py` & `mne-1.4.2/mne/viz/tests/test_circle.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_epochs.py` & `mne-1.4.2/mne/viz/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_evoked.py` & `mne-1.4.2/mne/viz/tests/test_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_ica.py` & `mne-1.4.2/mne/viz/tests/test_ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_misc.py` & `mne-1.4.2/mne/viz/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_montage.py` & `mne-1.4.2/mne/viz/tests/test_montage.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_proj.py` & `mne-1.4.2/mne/viz/tests/test_proj.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_raw.py` & `mne-1.4.2/mne/viz/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_scraper.py` & `mne-1.4.2/mne/viz/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_topo.py` & `mne-1.4.2/mne/viz/tests/test_topo.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_topomap.py` & `mne-1.4.2/mne/viz/tests/test_topomap.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/tests/test_utils.py` & `mne-1.4.2/mne/viz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/topo.py` & `mne-1.4.2/mne/viz/topo.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/topomap.py` & `mne-1.4.2/mne/viz/topomap.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne/viz/utils.py` & `mne-1.4.2/mne/viz/utils.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/mne.egg-info/PKG-INFO` & `mne-1.4.2/mne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne
-Version: 1.4.1
+Version: 1.4.2
 Summary: MNE-Python project for MEG and EEG data analysis.
 Home-page: https://mne.tools/dev/
 Download-URL: http://github.com/mne-tools/mne-python
 Maintainer: Alexandre Gramfort
 Maintainer-email: alexandre.gramfort@inria.fr
 License: BSD-3-Clause
 Project-URL: Homepage, https://mne.tools/
```

### Comparing `mne-1.4.1/mne.egg-info/SOURCES.txt` & `mne-1.4.2/mne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/pyproject.toml` & `mne-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/requirements.txt` & `mne-1.4.2/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 tqdm
 pooch>=1.5
 decorator
 h5io
 packaging
 pymatreader
 qtpy
-PySide6!=6.3.0,!=6.4.0,!=6.4.0.1,!=6.5.0  # incompat with Matplotlib 3.6.1 and qtpy
+PySide6!=6.5.1
 pyobjc-framework-Cocoa>=5.2.0; platform_system=="Darwin"
 sip
 scikit-learn
 nibabel
 openmeeg>=2.5.5
 numba
 h5py
```

### Comparing `mne-1.4.1/requirements_doc.txt` & `mne-1.4.2/requirements_doc.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/setup.py` & `mne-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import os.path as op
 
 from setuptools import setup
 
 
 if "SETUPTOOLS_SCM_PRETEND_VERSION" not in os.environ:
-    os.environ["SETUPTOOLS_SCM_PRETEND_VERSION"] = "1.4.1"
+    os.environ["SETUPTOOLS_SCM_PRETEND_VERSION"] = "1.4.2"
 
 
 def parse_requirements_file(fname):
     requirements = list()
     with open(fname, "r") as fid:
         for line in fid:
             req = line.strip()
```

### Comparing `mne-1.4.1/tutorials/README.txt` & `mne-1.4.2/tutorials/README.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/clinical/20_seeg.py` & `mne-1.4.2/tutorials/clinical/20_seeg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/clinical/30_ecog.py` & `mne-1.4.2/tutorials/clinical/30_ecog.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/clinical/60_sleep.py` & `mne-1.4.2/tutorials/clinical/60_sleep.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/clinical/README.txt` & `mne-1.4.2/tutorials/clinical/README.txt`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/10_epochs_overview.py` & `mne-1.4.2/tutorials/epochs/10_epochs_overview.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/15_baseline_regression.py` & `mne-1.4.2/tutorials/epochs/15_baseline_regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/20_visualize_epochs.py` & `mne-1.4.2/tutorials/epochs/20_visualize_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/30_epochs_metadata.py` & `mne-1.4.2/tutorials/epochs/30_epochs_metadata.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/40_autogenerate_metadata.py` & `mne-1.4.2/tutorials/epochs/40_autogenerate_metadata.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/50_epochs_to_data_frame.py` & `mne-1.4.2/tutorials/epochs/50_epochs_to_data_frame.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/epochs/60_make_fixed_length_epochs.py` & `mne-1.4.2/tutorials/epochs/60_make_fixed_length_epochs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/evoked/10_evoked_overview.py` & `mne-1.4.2/tutorials/evoked/10_evoked_overview.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/evoked/20_visualize_evoked.py` & `mne-1.4.2/tutorials/evoked/20_visualize_evoked.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/evoked/30_eeg_erp.py` & `mne-1.4.2/tutorials/evoked/30_eeg_erp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/evoked/40_whitened.py` & `mne-1.4.2/tutorials/evoked/40_whitened.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/10_background_freesurfer.py` & `mne-1.4.2/tutorials/forward/10_background_freesurfer.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/20_source_alignment.py` & `mne-1.4.2/tutorials/forward/20_source_alignment.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/25_automated_coreg.py` & `mne-1.4.2/tutorials/forward/25_automated_coreg.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/30_forward.py` & `mne-1.4.2/tutorials/forward/30_forward.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/35_eeg_no_mri.py` & `mne-1.4.2/tutorials/forward/35_eeg_no_mri.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/50_background_freesurfer_mne.py` & `mne-1.4.2/tutorials/forward/50_background_freesurfer_mne.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/80_fix_bem_in_blender.py` & `mne-1.4.2/tutorials/forward/80_fix_bem_in_blender.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/forward/90_compute_covariance.py` & `mne-1.4.2/tutorials/forward/90_compute_covariance.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/10_overview.py` & `mne-1.4.2/tutorials/intro/10_overview.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/15_inplace.py` & `mne-1.4.2/tutorials/intro/15_inplace.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/20_events_from_raw.py` & `mne-1.4.2/tutorials/intro/20_events_from_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/30_info.py` & `mne-1.4.2/tutorials/intro/30_info.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/40_sensor_locations.py` & `mne-1.4.2/tutorials/intro/40_sensor_locations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/50_configure_mne.py` & `mne-1.4.2/tutorials/intro/50_configure_mne.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/intro/70_report.py` & `mne-1.4.2/tutorials/intro/70_report.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/10_stc_class.py` & `mne-1.4.2/tutorials/inverse/10_stc_class.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/20_dipole_fit.py` & `mne-1.4.2/tutorials/inverse/20_dipole_fit.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/30_mne_dspm_loreta.py` & `mne-1.4.2/tutorials/inverse/30_mne_dspm_loreta.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/35_dipole_orientations.py` & `mne-1.4.2/tutorials/inverse/35_dipole_orientations.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/40_mne_fixed_free.py` & `mne-1.4.2/tutorials/inverse/40_mne_fixed_free.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/50_beamformer_lcmv.py` & `mne-1.4.2/tutorials/inverse/50_beamformer_lcmv.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/60_visualize_stc.py` & `mne-1.4.2/tutorials/inverse/60_visualize_stc.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/70_eeg_mri_coords.py` & `mne-1.4.2/tutorials/inverse/70_eeg_mri_coords.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/80_brainstorm_phantom_elekta.py` & `mne-1.4.2/tutorials/inverse/80_brainstorm_phantom_elekta.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/85_brainstorm_phantom_ctf.py` & `mne-1.4.2/tutorials/inverse/85_brainstorm_phantom_ctf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/inverse/90_phantom_4DBTi.py` & `mne-1.4.2/tutorials/inverse/90_phantom_4DBTi.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/io/10_reading_meg_data.py` & `mne-1.4.2/tutorials/io/10_reading_meg_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/io/20_reading_eeg_data.py` & `mne-1.4.2/tutorials/io/20_reading_eeg_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/io/30_reading_fnirs_data.py` & `mne-1.4.2/tutorials/io/30_reading_fnirs_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/io/60_ctf_bst_auditory.py` & `mne-1.4.2/tutorials/io/60_ctf_bst_auditory.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/io/70_reading_eyetracking_data.py` & `mne-1.4.2/tutorials/io/70_reading_eyetracking_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/machine-learning/30_strf.py` & `mne-1.4.2/tutorials/machine-learning/30_strf.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/machine-learning/50_decoding.py` & `mne-1.4.2/tutorials/machine-learning/50_decoding.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/10_preprocessing_overview.py` & `mne-1.4.2/tutorials/preprocessing/10_preprocessing_overview.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/15_handling_bad_channels.py` & `mne-1.4.2/tutorials/preprocessing/15_handling_bad_channels.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/20_rejecting_bad_data.py` & `mne-1.4.2/tutorials/preprocessing/20_rejecting_bad_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/25_background_filtering.py` & `mne-1.4.2/tutorials/preprocessing/25_background_filtering.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/30_filtering_resampling.py` & `mne-1.4.2/tutorials/preprocessing/30_filtering_resampling.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/35_artifact_correction_regression.py` & `mne-1.4.2/tutorials/preprocessing/35_artifact_correction_regression.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/40_artifact_correction_ica.py` & `mne-1.4.2/tutorials/preprocessing/40_artifact_correction_ica.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/45_projectors_background.py` & `mne-1.4.2/tutorials/preprocessing/45_projectors_background.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/50_artifact_correction_ssp.py` & `mne-1.4.2/tutorials/preprocessing/50_artifact_correction_ssp.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/55_setting_eeg_reference.py` & `mne-1.4.2/tutorials/preprocessing/55_setting_eeg_reference.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/59_head_positions.py` & `mne-1.4.2/tutorials/preprocessing/59_head_positions.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/60_maxwell_filtering_sss.py` & `mne-1.4.2/tutorials/preprocessing/60_maxwell_filtering_sss.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/70_fnirs_processing.py` & `mne-1.4.2/tutorials/preprocessing/70_fnirs_processing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/80_opm_processing.py` & `mne-1.4.2/tutorials/preprocessing/80_opm_processing.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/preprocessing/90_eyetracking_data.py` & `mne-1.4.2/tutorials/preprocessing/90_eyetracking_data.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/raw/10_raw_overview.py` & `mne-1.4.2/tutorials/raw/10_raw_overview.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/raw/20_event_arrays.py` & `mne-1.4.2/tutorials/raw/20_event_arrays.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/raw/30_annotate_raw.py` & `mne-1.4.2/tutorials/raw/30_annotate_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/raw/40_visualize_raw.py` & `mne-1.4.2/tutorials/raw/40_visualize_raw.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/simulation/10_array_objs.py` & `mne-1.4.2/tutorials/simulation/10_array_objs.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/simulation/70_point_spread.py` & `mne-1.4.2/tutorials/simulation/70_point_spread.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/simulation/80_dics.py` & `mne-1.4.2/tutorials/simulation/80_dics.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/10_background_stats.py` & `mne-1.4.2/tutorials/stats-sensor-space/10_background_stats.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/20_erp_stats.py` & `mne-1.4.2/tutorials/stats-sensor-space/20_erp_stats.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/40_cluster_1samp_time_freq.py` & `mne-1.4.2/tutorials/stats-sensor-space/40_cluster_1samp_time_freq.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/50_cluster_between_time_freq.py` & `mne-1.4.2/tutorials/stats-sensor-space/50_cluster_between_time_freq.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/70_cluster_rmANOVA_time_freq.py` & `mne-1.4.2/tutorials/stats-sensor-space/70_cluster_rmANOVA_time_freq.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-sensor-space/75_cluster_ftest_spatiotemporal.py` & `mne-1.4.2/tutorials/stats-sensor-space/75_cluster_ftest_spatiotemporal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-source-space/20_cluster_1samp_spatiotemporal.py` & `mne-1.4.2/tutorials/stats-source-space/20_cluster_1samp_spatiotemporal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-source-space/30_cluster_ftest_spatiotemporal.py` & `mne-1.4.2/tutorials/stats-source-space/30_cluster_ftest_spatiotemporal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/stats-source-space/60_cluster_rmANOVA_spatiotemporal.py` & `mne-1.4.2/tutorials/stats-source-space/60_cluster_rmANOVA_spatiotemporal.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/time-freq/10_spectrum_class.py` & `mne-1.4.2/tutorials/time-freq/10_spectrum_class.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/time-freq/20_sensors_time_frequency.py` & `mne-1.4.2/tutorials/time-freq/20_sensors_time_frequency.py`

 * *Files identical despite different names*

### Comparing `mne-1.4.1/tutorials/time-freq/50_ssvep.py` & `mne-1.4.2/tutorials/time-freq/50_ssvep.py`

 * *Files identical despite different names*

