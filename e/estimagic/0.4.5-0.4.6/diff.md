# Comparing `tmp/estimagic-0.4.5.tar.gz` & `tmp/estimagic-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimagic-0.4.5.tar", last modified: Mon Apr 10 11:40:41 2023, max compression
+gzip compressed data, was "estimagic-0.4.6.tar", last modified: Mon Jun  5 15:44:53 2023, max compression
```

## Comparing `estimagic-0.4.5.tar` & `estimagic-0.4.6.tar`

### file list

```diff
@@ -1,196 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.663413 estimagic-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-10 11:40:30.000000 estimagic-0.4.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 11:40:30.000000 estimagic-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-10 11:40:30.000000 estimagic-0.4.5/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 11:40:30.000000 estimagic-0.4.5/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-10 11:40:30.000000 estimagic-0.4.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 11:40:30.000000 estimagic-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-10 11:40:30.000000 estimagic-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-10 11:40:41.687413 estimagic-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-10 11:40:30.000000 estimagic-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-10 11:40:30.000000 estimagic-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-10 11:40:41.687413 estimagic-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 11:40:30.000000 estimagic-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.663413 estimagic-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/src/estimagic/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/batch_evaluators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129111 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/cartis_roberts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/get_benchmark_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/more_wild.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/noise_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/process_benchmark_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/benchmarking/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/plot_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/run_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/dashboard/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/differentiation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42827 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/finite_differences.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/generate_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/differentiation/richardson_extrapolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimate_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimate_msm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/estimation_summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/estimation/msm_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.671413 estimagic-0.4.5/src/estimagic/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/criterion_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/diabetes.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/exam_points.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/logit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/numdiff_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/examples/sensitivity_probit_example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.675413 estimagic-0.4.5/src/estimagic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/bootstrap_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/ml_covs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/msm_covs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/inference/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.675413 estimagic-0.4.5/src/estimagic/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/load_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/read_from_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/read_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/logging/write_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.679413 estimagic-0.4.5/src/estimagic/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/algo_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/bhhh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/check_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/convergence_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/cyipopt_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/error_penalty.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/fides_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/get_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/history_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/internal_criterion_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/nag_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/nlopt_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimization_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    44428 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/optimize_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22737 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders.py
--rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders_auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pounders_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/process_multistart_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    38576 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/pygmo_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/scipy_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/simopt_optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.679413 estimagic-0.4.5/src/estimagic/optimization/subsolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30929 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39208 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/subsolvers/linear_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tao_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tiktak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.683413 estimagic-0.4.5/src/estimagic/optimization/tranquilo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/acceptance_decision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/acceptance_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/adjust_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/aggregate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/estimate_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/filter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/get_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/handle_infinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/poisedness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/process_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/rho_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/solve_subproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/tranquilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/wrap_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/optimization/tranquilo/wrapped_subsolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/block_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/check_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/consolidate_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/constraint_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/kernel_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/parameter_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/parameter_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/process_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/process_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/scale_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/space_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/tree_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/parameters/tree_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/process_user_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/sensitivity/msm_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/shared/check_option_dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.687413 estimagic-0.4.5/src/estimagic/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/convergence_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/derivative_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/deviation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    58619 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/estimation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/history_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/lollipop_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/plotting_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/profile_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/slice_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-10 11:40:30.000000 estimagic-0.4.5/src/estimagic/visualization/visualize_tranquilo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:41.667413 estimagic-0.4.5/src/estimagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 11:40:41.000000 estimagic-0.4.5/src/estimagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.806179 estimagic-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.770179 estimagic-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.774179 estimagic-0.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.774179 estimagic-0.4.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.774179 estimagic-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-05 15:44:43.000000 estimagic-0.4.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-05 15:44:43.000000 estimagic-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-05 15:44:43.000000 estimagic-0.4.6/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-05 15:44:43.000000 estimagic-0.4.6/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-05 15:44:43.000000 estimagic-0.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-05 15:44:43.000000 estimagic-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-05 15:44:43.000000 estimagic-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-05 15:44:53.806179 estimagic-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-05 15:44:43.000000 estimagic-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-05 15:44:43.000000 estimagic-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-05 15:44:53.810179 estimagic-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:44:43.000000 estimagic-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.770179 estimagic-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.778179 estimagic-0.4.6/src/estimagic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/batch_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.782179 estimagic-0.4.6/src/estimagic/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129235 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/cartis_roberts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/get_benchmark_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/more_wild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/noise_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/process_benchmark_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/benchmarking/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.782179 estimagic-0.4.6/src/estimagic/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/plot_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/run_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/dashboard/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.786179 estimagic-0.4.6/src/estimagic/differentiation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/differentiation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42827 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/differentiation/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/differentiation/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/differentiation/generate_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/differentiation/richardson_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.786179 estimagic-0.4.6/src/estimagic/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/estimation/estimate_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/estimation/estimate_msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/estimation/estimation_summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/estimation/msm_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.786179 estimagic-0.4.6/src/estimagic/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/criterion_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/diabetes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/exam_points.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/numdiff_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/examples/sensitivity_probit_example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.790179 estimagic-0.4.6/src/estimagic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/bootstrap_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/bootstrap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/bootstrap_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/bootstrap_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/ml_covs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/msm_covs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/inference/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.790179 estimagic-0.4.6/src/estimagic/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/load_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/read_from_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/read_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/logging/write_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.798179 estimagic-0.4.6/src/estimagic/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/algo_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/bhhh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/check_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/convergence_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/cyipopt_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/error_penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/fides_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/get_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/history_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/internal_criterion_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/nag_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/nlopt_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/optimization_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44428 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/optimize_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22737 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/pounders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/pounders_auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/pounders_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/process_multistart_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38576 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/pygmo_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/scipy_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/simopt_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.802179 estimagic-0.4.6/src/estimagic/optimization/subsolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/_steihaug_toint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/_trsbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30929 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/bntr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/gqtpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/subsolvers/linear_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/tao_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19703 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/tiktak.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/optimization/tranquilo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.806179 estimagic-0.4.6/src/estimagic/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/block_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/check_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/consolidate_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/constraint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/kernel_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/parameter_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/parameter_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/process_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/process_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/scale_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/space_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/tree_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/parameters/tree_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/process_user_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.806179 estimagic-0.4.6/src/estimagic/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/sensitivity/msm_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.806179 estimagic-0.4.6/src/estimagic/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/shared/check_option_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.806179 estimagic-0.4.6/src/estimagic/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/convergence_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/derivative_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/deviation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58619 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/estimation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/history_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/lollipop_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/plotting_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/profile_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-05 15:44:43.000000 estimagic-0.4.6/src/estimagic/visualization/slice_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:44:53.778179 estimagic-0.4.6/src/estimagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 15:44:53.000000 estimagic-0.4.6/src/estimagic.egg-info/top_level.txt
```

### Comparing `estimagic-0.4.5/.github/ISSUE_TEMPLATE/bug-report.md` & `estimagic-0.4.6/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/.github/ISSUE_TEMPLATE/enhancement.md` & `estimagic-0.4.6/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md` & `estimagic-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/.github/workflows/main.yml` & `estimagic-0.4.6/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
           - ubuntu-latest
         python-version:
-          - '3.8'
           - '3.9'
           - '3.10'
+          - '3.11'
     steps:
       - uses: actions/checkout@v3
       - name: create build environment
         uses: mamba-org/provision-with-micromamba@main
         with:
           environment-file: ./.envs/testenv-linux.yml
           environment-name: estimagic
@@ -50,17 +50,17 @@
     strategy:
       fail-fast: false
       matrix:
         os:
           - macos-latest
           - windows-latest
         python-version:
-          - '3.8'
           - '3.9'
           - '3.10'
+          - '3.11'
     steps:
       - uses: actions/checkout@v3
       - name: create build environment
         uses: mamba-org/provision-with-micromamba@main
         with:
           environment-file: ./.envs/testenv-others.yml
           environment-name: estimagic
```

### Comparing `estimagic-0.4.5/.github/workflows/publish-to-pypi.yml` & `estimagic-0.4.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/.gitignore` & `estimagic-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/CHANGES.md` & `estimagic-0.4.6/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 # Changes
 
 This is a record of all past estimagic releases and what went into them in reverse
 chronological order. We follow [semantic versioning](https://semver.org/) and all
 releases are available on [Anaconda.org](https://anaconda.org/OpenSourceEconomics/estimagic).
 
+Following the [scientific python guidelines](https://scientific-python.org/specs/spec-0000/)
+we drop the official support for Python 3.8.
+
+
+## 0.4.6
+
+This release drastically improves the optimizer benchmarking capabilities, especially
+with noisy functions and parallel optimizers. It makes tranquilo and numba optional
+dependencies and is the first version of estimagic to be compatible with Python
+3.11.
+
+
+- {gh}`464` Makes tranquilo and numba optional dependencies ({ghuser}`janosg`)
+- {gh}`461` Updates docstrings for procss_benchmark_results ({ghuser}`segsell`)
+- {gh}`460` Fixes several bugs in the processing of benchmark results with noisy
+  functions ({ghuser}`janosg`)
+- {gh}`459` Prepares benchmarking functionality for parallel optimizers
+  ({ghuser}`mpetrosian` and {ghuser}`janosg`)
+- {gh}`457` Removes some unused files ({ghuser}`segsell`)
+- {gh}`455` Improves a local pre-commit hook ({ghuser}`ChristianZimpelmann`)
+
 
 ## 0.4.5
 
 - {gh}`379` Improves the estimation table ({ghuser}`ChristianZimpelmann`)
 - {gh}`445` fixes line endings in local pre-commit hook ({ghuser}`ChristianZimpelmann`)
 - {gh}`443`, {gh}`444`, {gh}`445`, {gh}`446`, {gh}`448` and {gh}`449` are a major
   refactoring of tranquilo ({ghuser}`timmens` and {ghuser}`janosg`)
```

### Comparing `estimagic-0.4.5/CITATION` & `estimagic-0.4.6/CITATION`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/CODE_OF_CONDUCT.md` & `estimagic-0.4.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/LICENSE` & `estimagic-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/MANIFEST.in` & `estimagic-0.4.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/PKG-INFO` & `estimagic-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimagic
-Version: 0.4.5
+Version: 0.4.6
 Summary: Tools to solve difficult numerical optimization problems.
 Home-page: https://github.com/OpenSourceEconomics/estimagic
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
 Classifier: Development Status :: 4 - Beta
```

### Comparing `estimagic-0.4.5/README.md` & `estimagic-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/pyproject.toml` & `estimagic-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     "ignore:Standard matrix inversion failed due to LinAlgError",
     "ignore:Tranquilo is extremely experimental",
     "ignore:delta_grad == 0.0",
     "ignore:Widget._active_widgets is deprecated",
     "ignore:Widget._widget_types is deprecated",
     "ignore:Widget.widget_types is deprecated",
     "ignore:Widget.widgets is deprecated",
+    "ignore:Parallelization together with",
 ]
 addopts = ["--doctest-modules"]
 markers = [
     "wip: Tests that are work-in-progress.",
     "slow: Tests that take a long time to run and are skipped in continuous integration.",
     "jax: Tests that require jax to be installed and are skipped on non-Linux systems.",
 ]
```

### Comparing `estimagic-0.4.5/setup.cfg` & `estimagic-0.4.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 [options]
 packages = find:
 install_requires = 
 	bokeh<=2.4.3
 	click
 	cloudpickle
 	joblib
-	numba
 	numpy>=1.17.0
 	pandas
 	plotly
 	pybaum>=0.1.2
 	scipy>=1.2.1
 	sqlalchemy>=1.3
 python_requires = >=3.8
```

### Comparing `estimagic-0.4.5/src/estimagic/__init__.py` & `estimagic-0.4.6/src/estimagic/__init__.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/batch_evaluators.py` & `estimagic-0.4.6/src/estimagic/batch_evaluators.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/benchmarking/cartis_roberts.py` & `estimagic-0.4.6/src/estimagic/benchmarking/cartis_roberts.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,24 @@
 - on sources cited in the SIF files or,
 - where available, on AMPL implementaions available here:
 - https://vanderbei.princeton.edu/ampl/nlmodels/cute/index.html
 
 """
 from functools import partial
 
-from numba import njit
 import numpy as np
+from estimagic.config import IS_NUMBA_INSTALLED
+
+if IS_NUMBA_INSTALLED:
+    from numba import njit
+else:
+
+    def njit(func):
+        return func
+
 
 from estimagic.benchmarking.more_wild import (
     brown_almost_linear,
     linear_full_rank,
     linear_rank_one,
     watson,
 )
```

### Comparing `estimagic-0.4.5/src/estimagic/benchmarking/get_benchmark_problems.py` & `estimagic-0.4.6/src/estimagic/benchmarking/get_benchmark_problems.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         exclude = set(exclude)
 
     rng = get_rng(seed)
     raw_problems = _get_raw_problems(name)
 
     raw_problems = {k: v for k, v in raw_problems.items() if k not in exclude}
 
+    is_noisy = bool(additive_noise or multiplicative_noise)
+
     if additive_noise:
         additive_options = _process_noise_options(additive_noise_options, False)
     else:
         additive_options = None
 
     if multiplicative_noise:
         multiplicative_options = _process_noise_options(
@@ -110,18 +112,21 @@
             multiplicative_options=multiplicative_options,
             scaling_options=scaling_options,
             rng=rng,
         )
 
         problems[name] = {
             "inputs": inputs,
+            "noise_free_criterion": specification["criterion"],
             "solution": _create_problem_solution(
                 specification, scaling_options=scaling_options
             ),
+            "noisy": is_noisy,
             "info": specification.get("info", {}),
+            "start_criterion": specification["start_criterion"],
         }
 
     return problems
 
 
 def _get_raw_problems(name):
     if name == "more_wild":
```

### Comparing `estimagic-0.4.5/src/estimagic/benchmarking/more_wild.py` & `estimagic-0.4.6/src/estimagic/benchmarking/more_wild.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/benchmarking/noise_distributions.py` & `estimagic-0.4.6/src/estimagic/benchmarking/noise_distributions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/benchmarking/run_benchmark.py` & `estimagic-0.4.6/src/estimagic/benchmarking/run_benchmark.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 - Add other benchmark sets:
     - finish medium scale problems from https://arxiv.org/pdf/1710.11005.pdf, Page 34.
     - add scalar problems from https://github.com/AxelThevenot
 - Add option for deterministic noise or wiggle.
 
 """
 import numpy as np
-import pandas as pd
-from pybaum import tree_just_flatten
 
 from estimagic import batch_evaluators
-from estimagic.optimization import AVAILABLE_ALGORITHMS
+from estimagic.algorithms import AVAILABLE_ALGORITHMS
 from estimagic.optimization.optimize import minimize
-from estimagic.optimization.optimize_result import OptimizeResult
+from pybaum import tree_just_flatten
 from estimagic.parameters.tree_registry import get_registry
 
 
 def run_benchmark(
     problems,
     optimize_options,
     *,
@@ -68,25 +66,41 @@
         )
     opt_options = _process_optimize_options(
         optimize_options,
         max_evals=max_criterion_evaluations,
         disable_convergence=disable_convergence,
     )
 
-    kwargs_list, names = _get_kwargs_list_and_names(problems, opt_options)
+    minimize_arguments, keys = _get_optimization_arguments_and_keys(
+        problems, opt_options
+    )
 
     raw_results = batch_evaluator(
         func=minimize,
-        arguments=kwargs_list,
+        arguments=minimize_arguments,
         n_cores=n_cores,
         error_handling=error_handling,
         unpack_symbol="**",
     )
 
-    results = _get_results(names, raw_results, kwargs_list)
+    processing_arguments = []
+    for name, raw_result in zip(keys, raw_results):
+        processing_arguments.append(
+            {"optimize_result": raw_result, "problem": problems[name[0]]}
+        )
+
+    results = batch_evaluator(
+        func=_process_one_result,
+        arguments=processing_arguments,
+        n_cores=n_cores,
+        error_handling="raise",
+        unpack_symbol="**",
+    )
+
+    results = dict(zip(keys, results))
 
     return results
 
 
 def _process_optimize_options(raw_options, max_evals, disable_convergence):
     if not isinstance(raw_options, dict):
         dict_options = {}
@@ -123,15 +137,15 @@
             option["algo_options"] = default_algo_options
 
         out_options[name] = option
 
     return out_options
 
 
-def _get_kwargs_list_and_names(problems, opt_options):
+def _get_optimization_arguments_and_keys(problems, opt_options):
     kwargs_list = []
     names = []
 
     for prob_name, problem in problems.items():
         for option_name, options in opt_options.items():
             algo = options["algorithm"]
             if isinstance(algo, str):
@@ -150,41 +164,56 @@
             kwargs["algo_options"] = algo_options
             kwargs_list.append(kwargs)
             names.append((prob_name, option_name))
 
     return kwargs_list, names
 
 
-def _get_results(names, raw_results, kwargs_list):
-    registry = get_registry(extended=True)
-    results = {}
-
-    for name, result, inputs in zip(names, raw_results, kwargs_list):
-        if isinstance(result, OptimizeResult):
-            history = result.history
-            params_history = pd.DataFrame(
-                [tree_just_flatten(p, registry=registry) for p in history["params"]]
-            )
-            criterion_history = pd.Series(history["criterion"])
-            time_history = pd.Series(history["runtime"])
-        elif isinstance(result, str):
-            _criterion = inputs["criterion"]
-
-            params_history = pd.DataFrame(
-                tree_just_flatten(inputs["params"], registry=registry)
-            ).T
-            criterion_history = pd.Series(_criterion(inputs["params"])["value"])
+def _process_one_result(optimize_result, problem):
+    """Process the result of one optimization run.
 
-            time_history = pd.Series([np.inf])
-        else:
-            raise TypeError(
-                "'result' object is expected to be of type 'dict' or 'str'."
-            )
-
-        results[name] = {
-            "params_history": params_history,
-            "criterion_history": criterion_history,
-            "time_history": time_history,
-            "solution": result,
-        }
+    Args:
+        optimize_result (OptimizeResult): Result of one optimization run.
+        problem (dict): Problem specification.
 
-    return results
+    Returns:
+        dict: Processed result.
+
+    """
+    _registry = get_registry(extended=True)
+    _criterion = problem["noise_free_criterion"]
+    _start_x = problem["inputs"]["params"]
+    _start_crit_value = _criterion(_start_x)
+    if isinstance(_start_crit_value, np.ndarray):
+        _start_crit_value = (_start_crit_value**2).sum()
+    _is_noisy = problem["noisy"]
+    _solution_crit = problem["solution"]["value"]
+
+    # This will happen if the optimization raised an error
+    if isinstance(optimize_result, str):
+        params_history_flat = [tree_just_flatten(_start_x, registry=_registry)]
+        criterion_history = [_start_crit_value]
+        time_history = [np.inf]
+        batches_history = [0]
+    else:
+        history = optimize_result.history
+        params_history = history["params"]
+        params_history_flat = [
+            tree_just_flatten(p, registry=_registry) for p in params_history
+        ]
+        if _is_noisy:
+            criterion_history = np.array([_criterion(p) for p in params_history])
+            if criterion_history.ndim == 2:
+                criterion_history = (criterion_history**2).sum(axis=1)
+        else:
+            criterion_history = history["criterion"]
+        criterion_history = np.clip(criterion_history, _solution_crit, np.inf)
+        batches_history = history["batches"]
+        time_history = history["runtime"]
+
+    return {
+        "params_history": params_history_flat,
+        "criterion_history": criterion_history,
+        "time_history": time_history,
+        "batches_history": batches_history,
+        "solution": optimize_result,
+    }
```

### Comparing `estimagic-0.4.5/src/estimagic/cli.py` & `estimagic-0.4.6/src/estimagic/cli.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/config.py` & `estimagic-0.4.6/src/estimagic/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,30 @@
     import simopt  # noqa: F401
 except ImportError:
     IS_SIMOPT_INSTALLED = False
 else:
     IS_SIMOPT_INSTALLED = True
 
 
+try:
+    import tranquilo  # noqa: F401
+except ImportError:
+    IS_TRANQUILO_INSTALLED = False
+else:
+    IS_TRANQUILO_INSTALLED = True
+
+
+try:
+    import numba  # noqa: F401
+except ImportError:
+    IS_NUMBA_INSTALLED = False
+else:
+    IS_NUMBA_INSTALLED = True
+
+
 # =================================================================================
 # Dashboard Defaults
 # =================================================================================
 
 Y_RANGE_PADDING = 0.05
 Y_RANGE_PADDING_UNITS = "absolute"
 PLOT_WIDTH = 750
```

### Comparing `estimagic-0.4.5/src/estimagic/dashboard/callbacks.py` & `estimagic-0.4.6/src/estimagic/dashboard/callbacks.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/dashboard/colors.py` & `estimagic-0.4.6/src/estimagic/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/dashboard/dashboard_app.py` & `estimagic-0.4.6/src/estimagic/dashboard/dashboard_app.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/dashboard/plot_functions.py` & `estimagic-0.4.6/src/estimagic/dashboard/plot_functions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/dashboard/run_dashboard.py` & `estimagic-0.4.6/src/estimagic/dashboard/run_dashboard.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/decorators.py` & `estimagic-0.4.6/src/estimagic/decorators.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/differentiation/derivatives.py` & `estimagic-0.4.6/src/estimagic/differentiation/derivatives.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,15 +719,15 @@
     df = df.set_index(["method", "num_term", "dim_x", "dim_f"])
     return df
 
 
 def _convert_evals_to_numpy(
     raw_evals, key, registry, is_scalar_out=False, is_vector_out=False
 ):
-    """harmonize the output of the function evaluations.
+    """Harmonize the output of the function evaluations.
 
     The raw_evals might contain dictionaries of which we only need one entry, scalar
     np.nan where we need arrays filled with np.nan or pandas objects. The processed
     evals only contain numpy arrays.
 
     """
     # get rid of dictionaries
```

### Comparing `estimagic-0.4.5/src/estimagic/differentiation/finite_differences.py` & `estimagic-0.4.6/src/estimagic/differentiation/finite_differences.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/differentiation/generate_steps.py` & `estimagic-0.4.6/src/estimagic/differentiation/generate_steps.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/differentiation/richardson_extrapolation.py` & `estimagic-0.4.6/src/estimagic/differentiation/richardson_extrapolation.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/estimation/estimate_ml.py` & `estimagic-0.4.6/src/estimagic/estimation/estimate_ml.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/estimation/estimate_msm.py` & `estimagic-0.4.6/src/estimagic/estimation/estimate_msm.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/estimation/msm_weighting.py` & `estimagic-0.4.6/src/estimagic/estimation/msm_weighting.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/examples/criterion_functions.py` & `estimagic-0.4.6/src/estimagic/examples/criterion_functions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/examples/diabetes.csv` & `estimagic-0.4.6/src/estimagic/examples/diabetes.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/examples/exam_points.csv` & `estimagic-0.4.6/src/estimagic/examples/exam_points.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/examples/logit.py` & `estimagic-0.4.6/src/estimagic/examples/logit.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/examples/numdiff_functions.py` & `estimagic-0.4.6/src/estimagic/examples/numdiff_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Functions with known gradients, jacobians or hessians.
 
 All functions take a numpy array with parameters as their first argument.
 
 Example inputs for the binary choice functions are in binary_choice_inputs.pickle. They
 come from the statsmodels documentation:
-
 https://tinyurl.com/y4x67vwl
 We pickled them so we don't need statsmodels as a dependency.
 
 """
 import numpy as np
 from scipy.stats import norm
```

### Comparing `estimagic-0.4.5/src/estimagic/examples/sensitivity_probit_example_data.csv` & `estimagic-0.4.6/src/estimagic/examples/sensitivity_probit_example_data.csv`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/exceptions.py` & `estimagic-0.4.6/src/estimagic/exceptions.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/bootstrap.py` & `estimagic-0.4.6/src/estimagic/inference/bootstrap.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/bootstrap_ci.py` & `estimagic-0.4.6/src/estimagic/inference/bootstrap_ci.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/bootstrap_helpers.py` & `estimagic-0.4.6/src/estimagic/inference/bootstrap_helpers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/bootstrap_outcomes.py` & `estimagic-0.4.6/src/estimagic/inference/bootstrap_outcomes.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/bootstrap_samples.py` & `estimagic-0.4.6/src/estimagic/inference/bootstrap_samples.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         n_draws=n_draws,
     )
     datasets = _get_bootstrap_samples_from_indices(data=data, bootstrap_indices=indices)
     return datasets
 
 
 def _get_bootstrap_samples_from_indices(data, bootstrap_indices):
-    """convert bootstrap indices into actual bootstrap samples.
+    """Convert bootstrap indices into actual bootstrap samples.
 
     Args:
         data (pandas.DataFrame): original dataset.
         bootstrap_indices (list): List with numpy arrays containing positional indices
             of observations in data.
 
     Returns:
```

### Comparing `estimagic-0.4.5/src/estimagic/inference/ml_covs.py` & `estimagic-0.4.6/src/estimagic/inference/ml_covs.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/msm_covs.py` & `estimagic-0.4.6/src/estimagic/inference/msm_covs.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/inference/shared.py` & `estimagic-0.4.6/src/estimagic/inference/shared.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/logging/create_tables.py` & `estimagic-0.4.6/src/estimagic/logging/create_tables.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/logging/load_database.py` & `estimagic-0.4.6/src/estimagic/logging/load_database.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/logging/read_from_database.py` & `estimagic-0.4.6/src/estimagic/logging/read_from_database.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/logging/read_log.py` & `estimagic-0.4.6/src/estimagic/logging/read_log.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/logging/write_to_database.py` & `estimagic-0.4.6/src/estimagic/logging/write_to_database.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/__init__.py` & `estimagic-0.4.6/src/estimagic/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     neldermead,
     nlopt_optimizers,
     pounders,
     pygmo_optimizers,
     scipy_optimizers,
     simopt_optimizers,
     tao_optimizers,
+    tranquilo,
 )
-from estimagic.optimization.tranquilo import tranquilo
 
 MODULES = [
     cyipopt_optimizers,
     fides_optimizers,
     nag_optimizers,
     nlopt_optimizers,
     pygmo_optimizers,
```

### Comparing `estimagic-0.4.5/src/estimagic/optimization/algo_options.py` & `estimagic-0.4.6/src/estimagic/optimization/algo_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
 CONSTRAINTS_ABSOLUTE_TOLERANCE = 1e-5
 """float: Allowed tolerance of the equality and inequality constraints for values to be
 considered 'feasible'.
 
 """
 
-
 """
 -------------------------
 Trust Region Parameters
 -------------------------
 """
 
 TRUSTREGION_THRESHOLD_SUCCESSFUL = 0.1
```

### Comparing `estimagic-0.4.5/src/estimagic/optimization/bhhh.py` & `estimagic-0.4.6/src/estimagic/optimization/bhhh.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/check_arguments.py` & `estimagic-0.4.6/src/estimagic/optimization/check_arguments.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/convergence_report.py` & `estimagic-0.4.6/src/estimagic/optimization/convergence_report.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/cyipopt_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/cyipopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/error_penalty.py` & `estimagic-0.4.6/src/estimagic/optimization/error_penalty.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/fides_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/fides_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/get_algorithm.py` & `estimagic-0.4.6/src/estimagic/optimization/get_algorithm.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 from estimagic.batch_evaluators import process_batch_evaluator
 from estimagic.logging.read_from_database import (
     list_of_dicts_to_dict_of_lists,
 )
 from estimagic.logging.write_to_database import update_row
-from estimagic.optimization import ALL_ALGORITHMS
+from estimagic.algorithms import ALL_ALGORITHMS
 from estimagic.utilities import propose_alternatives
 
 
 def process_user_algorithm(algorithm):
     """Process the user specfied algorithm.
 
     If the algorithm is a callable, this function just reads out the algorithm_info
@@ -56,16 +56,21 @@
     algo_options,
     logging,
     database,
     collect_history,
 ):
     """Get algorithm-function with partialled options.
 
-    The resulting function only depends on ``x``,  the relevant criterion functions
-    and derivatives and ``step_id``.
+    The resulting function only depends on ``x``,  the relevant criterion functions,
+    derivatives and ``step_id``. The remaining options are partialled in.
+
+    Moreover, we add the following capabilities over the internal algorithms:
+    - log the algorithm progress in a database (if logging is True)
+    - collect the history of parameters and criterion values as well as runtime and
+      batch information.
 
     Args:
         algorithm (str or callable): String with the name of an algorithm or internal
             algorithm function.
         lower_bounds (np.ndarray): 1d numpy array with lower bounds.
         upper_bounds (np.ndarray): 1d numpy array with upper bounds.
         nonlinear_constraints (list[dict]): List of dictionaries, each containing the
@@ -94,22 +99,19 @@
     algorithm = partial(raw_algorithm, **internal_options)
 
     algorithm = _add_logging(
         algorithm,
         logging=logging,
         database=database,
     )
-
-    is_parallel = internal_options.get("n_cores") not in (None, 1)
+    is_parallel = algo_info.parallelizes
+    batch_size = internal_options.get("batch_size", internal_options.get("n_cores", 1))
 
     if collect_history and not algo_info.disable_history:
-        algorithm = _add_history_collection_via_criterion(algorithm)
-        if is_parallel:
-            algorithm = _add_history_collection_via_batch_evaluator(algorithm)
-        algorithm = _add_history_processing(algorithm, is_parallel)
+        algorithm = _add_history_collection(algorithm, is_parallel, batch_size)
 
     return algorithm
 
 
 def _add_logging(algorithm=None, *, logging=None, database=None):
     """Add logging of status to the algorithm."""
 
@@ -150,112 +152,133 @@
 
     if callable(algorithm):
         return decorator_add_logging_to_algorithm(algorithm)
     else:
         return decorator_add_logging_to_algorithm
 
 
-def _add_history_collection_via_criterion(algorithm):
-    """Partial a history container into all functions that define the optimization."""
+def _add_history_collection(algorithm, is_parallel, batch_size):
+    """Add history collection to the algorithm.
 
-    @functools.wraps(algorithm)
-    def wrapper_add_history_collection_via_criterion(**kwargs):
-        func_names = {"criterion", "derivative", "criterion_and_derivative"}
+    The history collection is done jointly be the internal criterion function and the
+    batch evaluator. Using the batch evaluator for history collection is necessary
+    for two reasons:
+    1. The batch information is only known inside the batch evaluator
+    2. The normal approach of appending information to a list that is partialled into
+       the internal criterion function breaks down when the batch evaluator pickles
+       the internal criterion function.
+
+    We make sure that optimizers that do some function evaluations via the batch
+    evaluator and others directly are handled correctly.
+
+    The interplay between the two methods for history collections is as follows:
+    - If the function is called directly, all relevant information is appended to a list
+      that is partialled into the internal criterion function.
+    - If the function is called via the batch evaluator, we signal this to the internal
+      criterion via the two arguments ``history_container`` (which is set to None) and
+      ``return_history_entry`` (which is set to True). The returned history entries
+      are then collected inside the batch evaluator and appended to the history
+      container after all evaluations are done.
+
+    Args:
+        algorithm (callable): The algorithm.
+        is_parallel (bool): Whether the algorithm can parallelize.
+
+    """
 
+    @functools.wraps(algorithm)
+    def algorithm_with_history_collection(**kwargs):
+        # initialize the shared history container
         container = []
 
+        # add history collection via the internal criterion functions
+        func_names = {"criterion", "derivative", "criterion_and_derivative"}
         _kwargs = kwargs.copy()
         for name in func_names:
             if name in kwargs:
                 _kwargs[name] = partial(kwargs[name], history_container=container)
 
+        # add history collection via the batch evaluator
+        if is_parallel:
+            raw_be = kwargs.get("batch_evaluator", "joblib")
+            batch_evaluator = process_batch_evaluator(raw_be)
+
+            _kwargs["batch_evaluator"] = _get_history_collecting_batch_evaluator(
+                batch_evaluator=batch_evaluator,
+                container=container,
+                batch_size=batch_size,
+            )
+
+        # call the algorithm
         out = algorithm(**_kwargs)
+
+        # add the history container to the algorithm output
         if "history" not in out:
             out["history"] = container
         else:
             out["history"] = out["history"] + container
-        return out
-
-    return wrapper_add_history_collection_via_criterion
-
 
-def _add_history_collection_via_batch_evaluator(algorithm):
-    """Wrap the batch_evaluator argument such that histories are collected."""
+        # process the history
+        out["history"] = _process_collected_history(out["history"])
 
-    @functools.wraps(algorithm)
-    def wrapper_add_history_collection_via_batch_evaluator(**kwargs):
-        raw_be = kwargs.get("batch_evaluator", "joblib")
-        batch_evaluator = process_batch_evaluator(raw_be)
-
-        container = []
-
-        @functools.wraps(batch_evaluator)
-        def wrapped_batch_evaluator(*args, **kwargs):
-            if args:
-                func = args[0]
-            else:
-                func = kwargs["func"]
+        return out
 
-            # find out if func is our internal criterion function
-            if isinstance(func, partial) and "history_container" in func.keywords:
-                # partial in None as history container to disable history collection via
-                # criterion function, which would not work with parallelization anyways
-                _func = partial(func, history_container=None, return_history_entry=True)
-
-                if args:
-                    _args = (_func, *args[1:])
-                    _kwargs = kwargs
-                else:
-                    _args = args
-                    _kwargs = kwargs.copy()
-                    _kwargs["func"] = _func
+    return algorithm_with_history_collection
 
-                raw_out = batch_evaluator(*_args, **_kwargs)
 
-                out = [tup[0] for tup in raw_out]
-                _hist = [tup[1] for tup in raw_out if tup[1] is not None]
+def _get_history_collecting_batch_evaluator(batch_evaluator, container, batch_size):
+    @functools.wraps(batch_evaluator)
+    def history_collecting_batch_evaluator(*args, **kwargs):
+        if args:
+            func = args[0]
+        else:
+            func = kwargs["func"]
 
-                container.extend(_hist)
+        # find out if func is our internal criterion function. This is
+        # necessary because an algorithm might use the batch evaluatior for
+        # other functions as well, but for those functions we do not want to
+        # (and cannot) collect a history.
+        if isinstance(func, partial) and "history_container" in func.keywords:
+            # partial in None as history container to disable history collection
+            # via criterion function, which would not work with parallelization
+            _func = partial(func, history_container=None, return_history_entry=True)
 
+            if args:
+                _args = (_func, *args[1:])
+                _kwargs = kwargs
             else:
-                out = batch_evaluator(*args, **kwargs)
+                _args = args
+                _kwargs = kwargs.copy()
+                _kwargs["func"] = _func
+
+            raw_out = batch_evaluator(*_args, **_kwargs)
+            out = [tup[0] for tup in raw_out]
+            _hist = [tup[1] for tup in raw_out if tup[1] is not None]
+            _start_batch = container[-1]["batches"] + 1 if container else 0
+            _offsets = np.arange(len(_hist)).repeat(batch_size)[: len(_hist)]
+            _batch_info = _offsets + _start_batch
+            for batch, hist_entry in zip(_batch_info, _hist):
+                hist_entry["batches"] = batch
 
-            return out
+            container.extend(_hist)
 
-        new_kwargs = kwargs.copy()
-        new_kwargs["batch_evaluator"] = wrapped_batch_evaluator
-
-        out = algorithm(**new_kwargs)
-
-        if "history" in out:
-            out["history"] = out["history"] + container
         else:
-            out["history"] = container
+            out = batch_evaluator(*args, **kwargs)
 
         return out
 
-    return wrapper_add_history_collection_via_batch_evaluator
+    return history_collecting_batch_evaluator
 
 
-def _add_history_processing(algorithm, parallelizes):
-    @functools.wraps(algorithm)
-    def wrapper_add_history_processing(**kwargs):
-        out = algorithm(**kwargs)
-        raw = out["history"]
-        if parallelizes:
-            raw = sorted(raw, key=lambda e: e["runtime"])
-        history = list_of_dicts_to_dict_of_lists(raw)
-        runtimes = np.array(history["runtime"])
-        runtimes -= runtimes[0]
-        history["runtime"] = runtimes.tolist()
-
-        out["history"] = history
-        return out
-
-    return wrapper_add_history_processing
+def _process_collected_history(raw):
+    history = list_of_dicts_to_dict_of_lists(raw)
+    runtimes = np.array(history["runtime"])
+    runtimes -= runtimes[0]
+    history["runtime"] = runtimes.tolist()
+    return history
 
 
 def _adjust_options_to_algorithm(
     algo_options,
     lower_bounds,
     upper_bounds,
     nonlinear_constraints,
```

### Comparing `estimagic-0.4.5/src/estimagic/optimization/history_tools.py` & `estimagic-0.4.6/src/estimagic/optimization/history_tools.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/internal_criterion_template.py` & `estimagic-0.4.6/src/estimagic/optimization/internal_criterion_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,21 @@
 
     if new_criterion is not None:
         hist_entry = {
             "params": current_params,
             "criterion": scalar_critval,
             "runtime": now,
         }
+        if history_container is not None:
+            if history_container:
+                _batch = history_container[-1]["batches"] + 1
+            else:
+                _batch = 0
+
+            hist_entry["batches"] = _batch
     else:
         hist_entry = None
 
     if history_container is not None and new_criterion is not None:
         history_container.append(hist_entry)
 
     if return_history_entry:
```

### Comparing `estimagic-0.4.5/src/estimagic/optimization/nag_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/nag_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/neldermead.py` & `estimagic-0.4.6/src/estimagic/optimization/neldermead.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/nlopt_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/nlopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/optimization_logging.py` & `estimagic-0.4.6/src/estimagic/optimization/optimization_logging.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/optimize.py` & `estimagic-0.4.6/src/estimagic/optimization/optimize.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/optimize_result.py` & `estimagic-0.4.6/src/estimagic/optimization/optimize_result.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/pounders.py` & `estimagic-0.4.6/src/estimagic/optimization/pounders.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/pounders_auxiliary.py` & `estimagic-0.4.6/src/estimagic/optimization/pounders_auxiliary.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/pounders_history.py` & `estimagic-0.4.6/src/estimagic/optimization/pounders_history.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/process_multistart_sample.py` & `estimagic-0.4.6/src/estimagic/optimization/process_multistart_sample.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/process_results.py` & `estimagic-0.4.6/src/estimagic/optimization/process_results.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/pygmo_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/pygmo_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/scipy_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/scipy_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/simopt_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/simopt_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_conjugate_gradient.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_steihaug_toint.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/_steihaug_toint.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/_trsbox.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/_trsbox.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/bntr.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/bntr.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/gqtpar.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/gqtpar.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/subsolvers/linear_subsolvers.py` & `estimagic-0.4.6/src/estimagic/optimization/subsolvers/linear_subsolvers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/tao_optimizers.py` & `estimagic-0.4.6/src/estimagic/optimization/tao_optimizers.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/optimization/tiktak.py` & `estimagic-0.4.6/src/estimagic/optimization/tiktak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """Functions for multi start optimization a la TikTak.
 
 TikTak (`Arnoud, Guvenen, and Kleineberg
 <https://www.nber.org/system/files/working_papers/w26340/w26340.pdf>`_)
 
-
-
-
-
-
-is an algorithm for solving global optimization problems. It performs local searches
+ is an algorithm for solving global optimization problems. It performs local searches
 from a set of carefully-selected points in the parameter space.
 
 First implemented in Python by Alisdair McKay (
-
 `GitHub Repository <https://github.com/amckay/TikTak>`_)
 
 """
 import warnings
 from functools import partial
 
 import numpy as np
```

### Comparing `estimagic-0.4.5/src/estimagic/parameters/block_trees.py` & `estimagic-0.4.6/src/estimagic/parameters/block_trees.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/check_constraints.py` & `estimagic-0.4.6/src/estimagic/parameters/check_constraints.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/consolidate_constraints.py` & `estimagic-0.4.6/src/estimagic/parameters/consolidate_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
     return fixed_value
 
 
 def _consolidate_bounds_with_equality_constraints(
     equality_constraints, lower_bounds, upper_bounds
 ):
-    """consolidate bounds with equality constraints.
+    """Consolidate bounds with equality constraints.
 
     Check that there are no incompatible bounds on equality constrained parameters and
     set the bounds for equal parameters to the strictest bound encountered on any of
     them.
 
     Args:
         equality_constraints (list): List of constraints of type "equality".
```

### Comparing `estimagic-0.4.5/src/estimagic/parameters/constraint_tools.py` & `estimagic-0.4.6/src/estimagic/parameters/constraint_tools.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/conversion.py` & `estimagic-0.4.6/src/estimagic/parameters/conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/kernel_transformations.py` & `estimagic-0.4.6/src/estimagic/parameters/kernel_transformations.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/nonlinear_constraints.py` & `estimagic-0.4.6/src/estimagic/parameters/nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/parameter_bounds.py` & `estimagic-0.4.6/src/estimagic/parameters/parameter_bounds.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/parameter_groups.py` & `estimagic-0.4.6/src/estimagic/parameters/parameter_groups.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/process_constraints.py` & `estimagic-0.4.6/src/estimagic/parameters/process_constraints.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/process_selectors.py` & `estimagic-0.4.6/src/estimagic/parameters/process_selectors.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/scale_conversion.py` & `estimagic-0.4.6/src/estimagic/parameters/scale_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/space_conversion.py` & `estimagic-0.4.6/src/estimagic/parameters/space_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/tree_conversion.py` & `estimagic-0.4.6/src/estimagic/parameters/tree_conversion.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/parameters/tree_registry.py` & `estimagic-0.4.6/src/estimagic/parameters/tree_registry.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/process_user_function.py` & `estimagic-0.4.6/src/estimagic/process_user_function.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/sensitivity/msm_sensitivity.py` & `estimagic-0.4.6/src/estimagic/sensitivity/msm_sensitivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from estimagic.exceptions import INVALID_SENSITIVITY_MSG
 from estimagic.inference.msm_covs import cov_robust
 from estimagic.inference.shared import process_pandas_arguments
 from estimagic.utilities import robust_inverse
 
 
 def calculate_sensitivity_to_bias(jac, weights):
-    """calculate the sensitivity to bias.
+    """Calculate the sensitivity to bias.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How strongly would the parameter estimates be
         biased if the kth moment was misspecified, i.e not zero in expectation?
 
     Args:
@@ -43,15 +43,15 @@
 
     return m1
 
 
 def calculate_fundamental_sensitivity_to_noise(
     jac, weights, moments_cov, params_cov_opt
 ):
-    """calculate the fundamental sensitivity to noise.
+    """Calculate the fundamental sensitivity to noise.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How much precision would be lost if the kth
         moment was subject to a little additional noise if the optimal weighting matrix
         is used?
 
@@ -100,15 +100,15 @@
 
     return e2
 
 
 def calculate_actual_sensitivity_to_noise(
     sensitivity_to_bias, weights, moments_cov, params_cov
 ):
-    """calculate the actual sensitivity to noise.
+    """Calculate the actual sensitivity to noise.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How much precision would be lost if the kth
         moment was subjet to a little additional noise if "weights" is used as
         weighting matrix?
 
@@ -155,15 +155,15 @@
     if names:
         e3 = pd.DataFrame(e3, index=names.get("params"), columns=names.get("moments"))
 
     return e3
 
 
 def calculate_actual_sensitivity_to_removal(jac, weights, moments_cov, params_cov):
-    """calculate the actual sensitivity to removal.
+    """Calculate the actual sensitivity to removal.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How much precision would be lost if the kth
         moment was excluded from the estimation if "weights" is used as weighting
         matrix?
 
@@ -207,15 +207,15 @@
     if names:
         e4 = pd.DataFrame(e4, index=names.get("params"), columns=names.get("moments"))
 
     return e4
 
 
 def calculate_fundamental_sensitivity_to_removal(jac, moments_cov, params_cov_opt):
-    """calculate the fundamental sensitivity to removal.
+    """Calculate the fundamental sensitivity to removal.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How much precision would be lost if the kth
         moment was excluded from the estimation with if the optimal weighting matrix is
         used?
 
@@ -265,15 +265,15 @@
     if names:
         e5 = pd.DataFrame(e5, index=names.get("params"), columns=names.get("moments"))
 
     return e5
 
 
 def calculate_sensitivity_to_weighting(jac, weights, moments_cov, params_cov):
-    """calculate the sensitivity to weighting.
+    """Calculate the sensitivity to weighting.
 
     The sensitivity measure is calculated for each parameter wrt each moment.
 
     It answers the following question: How would the precision change if the weight of
         the kth moment is increased a little?
 
     Args:
```

### Comparing `estimagic-0.4.5/src/estimagic/shared/check_option_dicts.py` & `estimagic-0.4.6/src/estimagic/shared/check_option_dicts.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/utilities.py` & `estimagic-0.4.6/src/estimagic/utilities.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/convergence_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/convergence_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import plotly.express as px
 import plotly.graph_objects as go
 
 from estimagic.benchmarking.process_benchmark_results import (
-    create_convergence_histories,
+    process_benchmark_results,
 )
 from estimagic.config import PLOTLY_TEMPLATE
 from estimagic.utilities import propose_alternatives
 from estimagic.visualization.plotting_utilities import create_grid_plot, create_ind_dict
 
 
 def convergence_plot(
@@ -31,19 +31,20 @@
     """Plot convergence of optimizers for a set of problems.
 
     This creates a grid of plots, showing the convergence of the different
     algorithms on each problem. The faster a line falls, the faster the algorithm
     improved on the problem. The algorithm converged where its line reaches 0
     (if normalize_distance is True) or the horizontal blue line labeled "true solution".
 
-    Each plot shows on the x axis the runtime_measure, which can be walltime or number
-    of evaluations. Each algorithm's convergence is a line in the plot. Convergence can
-    be measured by the criterion value of the particular time/evaluation. The
-    convergence can be made monotone (i.e. always taking the bast value so far) or
-    normalized such that the distance from the start to the true solution is one.
+    Each plot shows on the x axis the runtime_measure, which can be walltime, number
+    of evaluations or number of batches. Each algorithm's convergence is a line in the
+    plot. Convergence can be measured by the criterion value of the particular
+    time/evaluation. The convergence can be made monotone (i.e. always taking the bast
+    value so far) or normalized such that the distance from the start to the true
+    solution is one.
 
     Args:
         problems (dict): estimagic benchmarking problems dictionary. Keys are the
             problem names. Values contain information on the problem, including the
             solution value.
         results (dict): estimagic benchmarking results dictionary. Keys are
             tuples of the form (problem, algorithm), values are dictionaries of the
@@ -60,15 +61,15 @@
         distance_measure (str): One of "criterion", "parameter_distance".
         monotone (bool): If True the best found criterion value so far is plotted.
             If False the particular criterion evaluation of that time is used.
         normalize_distance (bool): If True the progress is scaled by the total distance
             between the start value and the optimal value, i.e. 1 means the algorithm
             is as far from the solution as the start value and 0 means the algorithm
             has reached the solution value.
-        runtime_measure (str): "n_evaluations" or "walltime".
+        runtime_measure (str): "n_evaluations", "walltime" or "n_batches".
         stopping_criterion (str): "x_and_y", "x_or_y", "x", "y" or None. If None, no
             clipping is done.
         x_precision (float or None): how close an algorithm must have gotten to the
             true parameter values (as percent of the Euclidean distance between start
             and solution parameters) before the criterion for clipping and convergence
             is fulfilled.
         y_precision (float or None): how close an algorithm must have gotten to the
@@ -82,15 +83,15 @@
         palette: The coloring palette for traces. Default is "qualitative.Plotly".
 
     Returns:
         plotly.Figure: The grid plot or dict of individual plots
 
     """
 
-    df, _ = create_convergence_histories(
+    df, _ = process_benchmark_results(
         problems=problems,
         results=results,
         stopping_criterion=stopping_criterion,
         x_precision=x_precision,
         y_precision=y_precision,
     )
 
@@ -134,26 +135,31 @@
         "monotone_parameter_distance": "Distance Between the Best Parameters So Far<br>"
         "and the Optimal Parameters",
     }
 
     x_labels = {
         "n_evaluations": "Number of Function Evaluations",
         "walltime": "Elapsed Time",
+        "n_batches": "Number of Batches",
     }
 
     # container for individual plots
     g_list = []
     # container for titles
     titles = []
 
     # creating data traces for plotting faceted/individual plots
     # dropping usage of palette for algoritms, but use the built in pallete
     for prob_name in remaining_problems:
         g_ind = []  # container for data for traces in individual plot
         to_plot = df[df["problem"] == prob_name]
+        if runtime_measure == "n_batches":
+            to_plot = (
+                to_plot.groupby(["algorithm", runtime_measure]).min().reset_index()
+            )
 
         for i, alg in enumerate(to_plot["algorithm"].unique()):
             temp = to_plot[to_plot["algorithm"] == alg]
             trace_1 = go.Scatter(
                 x=temp[runtime_measure],
                 y=temp[outcome],
                 mode="lines",
```

### Comparing `estimagic-0.4.5/src/estimagic/visualization/derivative_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/derivative_plot.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/deviation_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/deviation_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pandas as pd
 import plotly.express as px
 
 from estimagic.benchmarking.process_benchmark_results import (
-    create_convergence_histories,
+    process_benchmark_results,
 )
 from estimagic.config import PLOTLY_TEMPLATE
 
 
 def deviation_plot(
     problems,
     results,
     *,
+    runtime_measure="n_evaluations",
     distance_measure="criterion",
     monotone=True,
     template=PLOTLY_TEMPLATE,
 ):
     """Plot average convergence of optimizers for a set of problems.
 
     Returns aggregated version convergence plot, showing the convergence of the
@@ -31,67 +32,72 @@
         problems (dict): estimagic benchmarking problems dictionary. Keys are the
             problem names. Values contain information on the problem, including the
             solution value.
         results (dict): estimagic benchmarking results dictionary. Keys are
             tuples of the form (problem, algorithm), values are dictionaries of the
             collected information on the benchmark run, including 'criterion_history'
             and 'time_history'.
+        runtime_measure (str): One of "n_evaluations", "n_batches".
         distance_measure (str): One of "criterion", "parameter_distance".
         monotone (bool): If True the best found criterion value so far is plotted.
             If False the particular criterion evaluation of that time is used.
         template (str): The template for the figure. Default is "plotly_white".
 
     Returns:
         plotly.Figure
 
     """
-
-    df, _ = create_convergence_histories(
+    df, _ = process_benchmark_results(
         problems=problems,
         results=results,
         stopping_criterion="y",
         x_precision=1e-6,
         y_precision=1e-6,
     )
 
     outcome = f"{'monotone_' if monotone else ''}" + distance_measure + "_normalized"
     deviations = (
-        df.set_index(["problem", "algorithm", "n_evaluations"])[outcome]
+        df.groupby(["problem", "algorithm", runtime_measure])
+        .min()[outcome]
         .reindex(
             pd.MultiIndex.from_product(
                 [
                     df["problem"].unique(),
                     df["algorithm"].unique(),
-                    range(df["n_evaluations"].min(), df["n_evaluations"].max() + 1),
+                    range(df[runtime_measure].min(), df[runtime_measure].max() + 1),
                 ],
-                names=["problem", "algorithm", "n_evaluations"],
+                names=["problem", "algorithm", runtime_measure],
             )
         )
         .fillna(method="ffill")
         .reset_index()
     )
     average_deviations = (
-        deviations.groupby(["algorithm", "n_evaluations"])
+        deviations.groupby(["algorithm", runtime_measure])
         .mean(numeric_only=True)[outcome]
         .reset_index()
     )
-    fig = px.line(average_deviations, x="n_evaluations", y=outcome, color="algorithm")
+    fig = px.line(average_deviations, x=runtime_measure, y=outcome, color="algorithm")
 
     y_labels = {
         "criterion_normalized": "Share of Function Distance to Optimum<br>"
         "Missing From Current Criterion Value",
         "monotone_criterion_normalized": "Share of Function Distance to Optimum<br>"
         "Missing From Best So Far",
         "parameter_distance_normalized": "Share of Parameter Distance to Optimum<br>"
         "Missing From Current Parameters",
         "monotone_parameter_distance_normalized": "Share of the Parameter Distance "
         "to Optimum<br> Missing From the Best Parameters So Far",
     }
+    x_labels = {
+        "n_evaluations": "Numver of Function Evaluations",
+        "n_batches": "Number of Batches",
+    }
     fig.update_layout(
-        xaxis_title="Number of Function Evaluations",
+        xaxis_title=x_labels[runtime_measure],
         yaxis_title=y_labels[outcome],
         title=None,
         height=300,
         width=500,
         margin={"l": 10, "r": 10, "t": 30, "b": 10},
         template=template,
     )
```

### Comparing `estimagic-0.4.5/src/estimagic/visualization/estimation_table.py` & `estimagic-0.4.6/src/estimagic/visualization/estimation_table.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/history_plots.py` & `estimagic-0.4.6/src/estimagic/visualization/history_plots.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/lollipop_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/lollipop_plot.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/plotting_utilities.py` & `estimagic-0.4.6/src/estimagic/visualization/plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic/visualization/profile_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/profile_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
 from estimagic.benchmarking.process_benchmark_results import (
-    create_convergence_histories,
+    process_benchmark_results,
 )
 from estimagic.config import PLOTLY_TEMPLATE
 
 
 def profile_plot(
     problems,
     results,
@@ -42,15 +42,15 @@
         problems (dict): estimagic benchmarking problems dictionary. Keys are the
             problem names. Values contain information on the problem, including the
             solution value.
         results (dict): estimagic benchmarking results dictionary. Keys are
             tuples of the form (problem, algorithm), values are dictionaries of the
             collected information on the benchmark run, including 'criterion_history'
             and 'time_history'.
-        runtime_measure (str): "n_evaluations" or "walltime".
+        runtime_measure (str): "n_evaluations", "n_batches" or "walltime".
             This is the runtime until the desired convergence was reached by an
             algorithm. This is called performance measure by Moré and Wild (2009).
         normalize_runtime (bool): If True the runtime each algorithm needed for each
             problem is scaled by the time the fastest algorithm needed. If True, the
             resulting plot is what Moré and Wild (2009) called data profiles.
         stopping_criterion (str): one of "x_and_y", "x_or_y", "x", "y". Determines
             how convergence is determined from the two precisions.
@@ -68,21 +68,21 @@
         plotly.Figure
 
     """
     if stopping_criterion is None:
         raise ValueError(
             "You must specify a stopping criterion for the performance plot. "
         )
-    if runtime_measure not in ["walltime", "n_evaluations"]:
+    if runtime_measure not in ["walltime", "n_evaluations", "n_batches"]:
         raise ValueError(
             "Only 'walltime' or 'n_evaluations' are allowed as "
             f"runtime_measure. You specified {runtime_measure}."
         )
 
-    df, converged_info = create_convergence_histories(
+    df, converged_info = process_benchmark_results(
         problems=problems,
         results=results,
         stopping_criterion=stopping_criterion,
         x_precision=x_precision,
         y_precision=y_precision,
     )
 
@@ -111,16 +111,22 @@
             True,
         ): "Multiple of Minimal Number of Function Evaluations<br>"
         "Needed to Solve the Problem",
         (
             "walltime",
             True,
         ): "Multiple of Minimal Wall Time<br>Needed to Solve the Problem",
+        (
+            "n_batches",
+            True,
+        ): "Multiple of Minimal Number of Batches<br>"
+        "Needed to Solve the Problem",
         ("n_evaluations", False): "Number of Function Evaluations",
         ("walltime", False): "Wall Time Needed to Solve the Problem",
+        ("n_batches", False): "Number of Batches",
     }
 
     fig.update_layout(
         xaxis_title=xlabels[(runtime_measure, normalize_runtime)],
         yaxis_title="Share of Problems Solved",
         title=None,
         height=300,
@@ -135,15 +141,15 @@
 
 def _create_solution_times(df, runtime_measure, converged_info):
     """Find the solution time for each algorithm and problem.
 
     Args:
         df (pandas.DataFrame): contains 'problem', 'algorithm' and *runtime_measure*
             as columns.
-        runtime_measure (str): 'walltime' or 'n_evaluations'.
+        runtime_measure (str): 'walltime', 'n_batches' or 'n_evaluations'.
         converged_info (pandas.DataFrame): columns are the algorithms, index are the
             problems. The values are boolean and True when the algorithm arrived at
             the solution with the desired precision.
 
     Returns:
         solution_times (pandas.DataFrame): columns are algorithms, index are problems.
             The values are either the number of evaluations or the walltime each
```

### Comparing `estimagic-0.4.5/src/estimagic/visualization/slice_plot.py` & `estimagic-0.4.6/src/estimagic/visualization/slice_plot.py`

 * *Files identical despite different names*

### Comparing `estimagic-0.4.5/src/estimagic.egg-info/PKG-INFO` & `estimagic-0.4.6/src/estimagic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimagic
-Version: 0.4.5
+Version: 0.4.6
 Summary: Tools to solve difficult numerical optimization problems.
 Home-page: https://github.com/OpenSourceEconomics/estimagic
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: econometrics,statistics,estimation,extremum estimation,optimization,inference,numerical differentiation,finite differences,richardson extrapolation,derivative free optimization,method of simulated moments,maximum likelihood
 Classifier: Development Status :: 4 - Beta
```

### Comparing `estimagic-0.4.5/src/estimagic.egg-info/SOURCES.txt` & `estimagic-0.4.6/src/estimagic.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/ISSUE_TEMPLATE/enhancement.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/PULL_REQUEST_TEMPLATE/pull_request_template.md
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 src/estimagic/__init__.py
 src/estimagic/_version.py
+src/estimagic/algorithms.py
 src/estimagic/batch_evaluators.py
 src/estimagic/cli.py
 src/estimagic/config.py
 src/estimagic/decorators.py
 src/estimagic/exceptions.py
 src/estimagic/process_user_function.py
 src/estimagic/utilities.py
@@ -100,52 +101,21 @@
 src/estimagic/optimization/process_multistart_sample.py
 src/estimagic/optimization/process_results.py
 src/estimagic/optimization/pygmo_optimizers.py
 src/estimagic/optimization/scipy_optimizers.py
 src/estimagic/optimization/simopt_optimizers.py
 src/estimagic/optimization/tao_optimizers.py
 src/estimagic/optimization/tiktak.py
+src/estimagic/optimization/tranquilo.py
 src/estimagic/optimization/subsolvers/_conjugate_gradient.py
-src/estimagic/optimization/subsolvers/_conjugate_gradient_fast.py
 src/estimagic/optimization/subsolvers/_steihaug_toint.py
-src/estimagic/optimization/subsolvers/_steihaug_toint_fast.py
 src/estimagic/optimization/subsolvers/_trsbox.py
-src/estimagic/optimization/subsolvers/_trsbox_fast.py
 src/estimagic/optimization/subsolvers/bntr.py
-src/estimagic/optimization/subsolvers/bntr_fast.py
 src/estimagic/optimization/subsolvers/gqtpar.py
-src/estimagic/optimization/subsolvers/gqtpar_fast.py
 src/estimagic/optimization/subsolvers/linear_subsolvers.py
-src/estimagic/optimization/tranquilo/__init__.py
-src/estimagic/optimization/tranquilo/acceptance_decision.py
-src/estimagic/optimization/tranquilo/acceptance_sample_size.py
-src/estimagic/optimization/tranquilo/adjust_radius.py
-src/estimagic/optimization/tranquilo/aggregate_models.py
-src/estimagic/optimization/tranquilo/bounds.py
-src/estimagic/optimization/tranquilo/clustering.py
-src/estimagic/optimization/tranquilo/estimate_variance.py
-src/estimagic/optimization/tranquilo/filter_points.py
-src/estimagic/optimization/tranquilo/fit_models.py
-src/estimagic/optimization/tranquilo/geometry.py
-src/estimagic/optimization/tranquilo/get_component.py
-src/estimagic/optimization/tranquilo/handle_infinity.py
-src/estimagic/optimization/tranquilo/history.py
-src/estimagic/optimization/tranquilo/models.py
-src/estimagic/optimization/tranquilo/options.py
-src/estimagic/optimization/tranquilo/poisedness.py
-src/estimagic/optimization/tranquilo/process_arguments.py
-src/estimagic/optimization/tranquilo/region.py
-src/estimagic/optimization/tranquilo/rho_noise.py
-src/estimagic/optimization/tranquilo/sample_points.py
-src/estimagic/optimization/tranquilo/solve_subproblem.py
-src/estimagic/optimization/tranquilo/tranquilo.py
-src/estimagic/optimization/tranquilo/volume.py
-src/estimagic/optimization/tranquilo/weighting.py
-src/estimagic/optimization/tranquilo/wrap_criterion.py
-src/estimagic/optimization/tranquilo/wrapped_subsolvers.py
 src/estimagic/parameters/__init__.py
 src/estimagic/parameters/block_trees.py
 src/estimagic/parameters/check_constraints.py
 src/estimagic/parameters/consolidate_constraints.py
 src/estimagic/parameters/constraint_tools.py
 src/estimagic/parameters/conversion.py
 src/estimagic/parameters/kernel_transformations.py
@@ -165,9 +135,8 @@
 src/estimagic/visualization/derivative_plot.py
 src/estimagic/visualization/deviation_plot.py
 src/estimagic/visualization/estimation_table.py
 src/estimagic/visualization/history_plots.py
 src/estimagic/visualization/lollipop_plot.py
 src/estimagic/visualization/plotting_utilities.py
 src/estimagic/visualization/profile_plot.py
-src/estimagic/visualization/slice_plot.py
-src/estimagic/visualization/visualize_tranquilo.py
+src/estimagic/visualization/slice_plot.py
```

