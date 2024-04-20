# Comparing `tmp/phitter-0.0.4.tar.gz` & `tmp/phitter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phitter-0.0.4.tar", last modified: Fri Mar 29 01:10:02 2024, max compression
+gzip compressed data, was "phitter-0.0.5.tar", last modified: Sat Apr 20 07:39:06 2024, max compression
```

## Comparing `phitter-0.0.4.tar` & `phitter-0.0.5.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.073913 phitter-0.0.4/
--rw-rw-rw-   0        0        0     1121 2024-03-19 04:53:21.000000 phitter-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    17751 2024-03-29 01:10:02.071302 phitter-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    14785 2024-03-29 00:47:23.000000 phitter-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:01.607808 phitter-0.0.4/phitter/
--rw-rw-rw-   0        0        0      114 2024-03-29 01:09:33.000000 phitter-0.0.4/phitter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:01.649107 phitter-0.0.4/phitter/continuous/
--rw-rw-rw-   0        0        0     5472 2024-03-26 21:53:33.000000 phitter-0.0.4/phitter/continuous/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:01.994967 phitter-0.0.4/phitter/continuous/continuous_distributions/
--rw-rw-rw-   0        0        0     5110 2024-03-22 02:27:55.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/__init__.py
--rw-rw-rw-   0        0        0    11120 2024-03-27 17:42:14.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/alpha.py
--rw-rw-rw-   0        0        0     8025 2024-03-27 17:39:15.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/arcsine.py
--rw-rw-rw-   0        0        0     8360 2024-03-27 17:40:07.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/argus.py
--rw-rw-rw-   0        0        0    12142 2024-03-27 17:39:17.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/beta.py
--rw-rw-rw-   0        0        0     9621 2024-03-27 17:40:06.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/beta_prime.py
--rw-rw-rw-   0        0        0    10481 2024-03-27 17:40:06.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/beta_prime_4p.py
--rw-rw-rw-   0        0        0     8373 2024-03-27 17:40:05.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/bradford.py
--rw-rw-rw-   0        0        0     9720 2024-03-27 17:47:53.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/burr.py
--rw-rw-rw-   0        0        0    10020 2024-03-27 17:40:03.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/burr_4p.py
--rw-rw-rw-   0        0        0     7525 2024-03-27 17:40:04.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/cauchy.py
--rw-rw-rw-   0        0        0     6730 2024-03-27 17:40:02.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/chi_square.py
--rw-rw-rw-   0        0        0     8632 2024-03-27 17:40:03.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/chi_square_3p.py
--rw-rw-rw-   0        0        0    10529 2024-03-27 17:40:01.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/dagum.py
--rw-rw-rw-   0        0        0    10865 2024-03-27 17:40:00.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/dagum_4p.py
--rw-rw-rw-   0        0        0     7643 2024-03-27 17:40:00.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/erlang.py
--rw-rw-rw-   0        0        0     7930 2024-03-27 17:39:17.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/erlang_3p.py
--rw-rw-rw-   0        0        0     6420 2024-03-27 17:39:18.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/error_function.py
--rw-rw-rw-   0        0        0     6557 2024-03-27 19:03:37.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/exponential.py
--rw-rw-rw-   0        0        0     6992 2024-03-27 19:03:17.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/exponential_2p.py
--rw-rw-rw-   0        0        0     7918 2024-03-27 17:39:19.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/f.py
--rw-rw-rw-   0        0        0    10656 2024-03-27 17:39:56.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/f_4p.py
--rw-rw-rw-   0        0        0     8636 2024-03-27 17:39:59.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/fatigue_life.py
--rw-rw-rw-   0        0        0     8647 2024-03-27 17:39:57.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/folded_normal.py
--rw-rw-rw-   0        0        0     8178 2024-03-27 17:39:21.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/frechet.py
--rw-rw-rw-   0        0        0     7862 2024-03-27 17:39:21.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/gamma.py
--rw-rw-rw-   0        0        0     8106 2024-03-27 17:39:57.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/gamma_3p.py
--rw-rw-rw-   0        0        0     8863 2024-03-27 17:39:23.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_extreme_value.py
--rw-rw-rw-   0        0        0     9515 2024-03-27 17:39:23.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_gamma.py
--rw-rw-rw-   0        0        0    10277 2024-03-27 17:49:37.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_gamma_4p.py
--rw-rw-rw-   0        0        0     9468 2024-03-27 17:39:24.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_logistic.py
--rw-rw-rw-   0        0        0     7604 2024-03-27 17:39:25.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_normal.py
--rw-rw-rw-   0        0        0     9827 2024-03-27 17:39:24.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_pareto.py
--rw-rw-rw-   0        0        0     7376 2024-03-27 17:39:26.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/gibrat.py
--rw-rw-rw-   0        0        0     7280 2024-03-27 17:39:26.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/gumbel_left.py
--rw-rw-rw-   0        0        0     7283 2024-03-27 17:39:28.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/gumbel_right.py
--rw-rw-rw-   0        0        0     6859 2024-03-27 17:39:27.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/half_normal.py
--rw-rw-rw-   0        0        0     6685 2024-03-27 17:39:55.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/hyperbolic_secant.py
--rw-rw-rw-   0        0        0    11375 2024-03-27 19:06:08.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gamma.py
--rw-rw-rw-   0        0        0    10025 2024-03-27 17:39:30.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gamma_3p.py
--rw-rw-rw-   0        0        0     6617 2024-03-27 17:39:30.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gaussian.py
--rw-rw-rw-   0        0        0     7659 2024-03-27 17:39:31.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gaussian_3p.py
--rw-rw-rw-   0        0        0     9698 2024-03-27 17:39:32.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/johnson_sb.py
--rw-rw-rw-   0        0        0     9343 2024-03-27 17:39:33.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/johnson_su.py
--rw-rw-rw-   0        0        0    10223 2024-03-27 17:39:33.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/kumaraswamy.py
--rw-rw-rw-   0        0        0     5928 2024-03-27 17:39:34.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/laplace.py
--rw-rw-rw-   0        0        0     7748 2024-03-27 17:39:54.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/levy.py
--rw-rw-rw-   0        0        0    10270 2024-03-27 17:39:35.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/loggamma.py
--rw-rw-rw-   0        0        0     6724 2024-03-27 17:39:35.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/logistic.py
--rw-rw-rw-   0        0        0    10177 2024-03-27 17:39:53.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/loglogistic.py
--rw-rw-rw-   0        0        0     9435 2024-03-27 17:39:36.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/loglogistic_3p.py
--rw-rw-rw-   0        0        0     7197 2024-03-27 20:02:27.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/lognormal.py
--rw-rw-rw-   0        0        0     8497 2024-03-27 17:39:51.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/maxwell.py
--rw-rw-rw-   0        0        0     7955 2024-03-27 17:39:38.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/moyal.py
--rw-rw-rw-   0        0        0     7858 2024-03-27 17:39:38.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/nakagami.py
--rw-rw-rw-   0        0        0     9109 2024-03-27 17:39:52.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_chi_square.py
--rw-rw-rw-   0        0        0    11530 2024-03-27 17:39:40.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_f.py
--rw-rw-rw-   0        0        0    12039 2024-03-27 17:39:39.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_t_student.py
--rw-rw-rw-   0        0        0     6689 2024-03-27 17:39:53.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/normal.py
--rw-rw-rw-   0        0        0    10542 2024-03-27 17:39:50.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/pareto_first_kind.py
--rw-rw-rw-   0        0        0    10345 2024-03-27 17:39:41.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/pareto_second_kind.py
--rw-rw-rw-   0        0        0     9742 2024-03-27 17:39:41.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/pert.py
--rw-rw-rw-   0        0        0    10412 2024-03-27 17:39:49.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/power_function.py
--rw-rw-rw-   0        0        0     7319 2024-03-27 17:39:50.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/rayleigh.py
--rw-rw-rw-   0        0        0     7303 2024-03-27 17:39:42.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/reciprocal.py
--rw-rw-rw-   0        0        0    11079 2024-03-27 17:39:42.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/rice.py
--rw-rw-rw-   0        0        0     6863 2024-03-27 17:39:48.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/semicircular.py
--rw-rw-rw-   0        0        0     7161 2024-03-27 20:05:17.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/t_student.py
--rw-rw-rw-   0        0        0     7663 2024-03-27 20:04:09.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/t_student_3p.py
--rw-rw-rw-   0        0        0    10045 2024-03-27 17:39:47.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/trapezoidal.py
--rw-rw-rw-   0        0        0     9881 2024-03-27 17:39:43.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/triangular.py
--rw-rw-rw-   0        0        0     6398 2024-03-27 17:39:44.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/uniform.py
--rw-rw-rw-   0        0        0     8584 2024-03-27 17:39:46.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/weibull.py
--rw-rw-rw-   0        0        0     8993 2024-03-27 17:39:46.000000 phitter-0.0.4/phitter/continuous/continuous_distributions/weibull_3p.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.003031 phitter-0.0.4/phitter/continuous/continuous_measures/
--rw-rw-rw-   0        0        0       54 2024-03-01 00:26:16.000000 phitter-0.0.4/phitter/continuous/continuous_measures/__init__.py
--rw-rw-rw-   0        0        0     5748 2024-03-20 01:28:03.000000 phitter-0.0.4/phitter/continuous/continuous_measures/continuous_measures.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.015764 phitter-0.0.4/phitter/continuous/continuous_statistical_tests/
--rw-rw-rw-   0        0        0      273 2024-02-29 22:48:49.000000 phitter-0.0.4/phitter/continuous/continuous_statistical_tests/__init__.py
--rw-rw-rw-   0        0        0     3676 2024-03-22 02:27:55.000000 phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_anderson_darling.py
--rw-rw-rw-   0        0        0     3354 2024-03-22 02:27:55.000000 phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_chi_square.py
--rw-rw-rw-   0        0        0     3060 2024-03-22 02:27:55.000000 phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_kolmogorov_smirnov.py
--rw-rw-rw-   0        0        0    20391 2024-03-27 17:57:49.000000 phitter-0.0.4/phitter/continuous/phitter_continuous.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.022843 phitter-0.0.4/phitter/discrete/
--rw-rw-rw-   0        0        0      850 2024-03-26 22:02:58.000000 phitter-0.0.4/phitter/discrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.052428 phitter-0.0.4/phitter/discrete/discrete_distributions/
--rw-rw-rw-   0        0        0      581 2024-03-22 02:27:56.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/__init__.py
--rw-rw-rw-   0        0        0     6450 2024-03-27 17:54:15.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/bernoulli.py
--rw-rw-rw-   0        0        0     6567 2024-03-27 17:54:16.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/binomial.py
--rw-rw-rw-   0        0        0     6233 2024-03-27 17:54:17.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/geometric.py
--rw-rw-rw-   0        0        0     8716 2024-03-27 17:54:17.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/hypergeometric.py
--rw-rw-rw-   0        0        0     7262 2024-03-27 17:54:17.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/logarithmic.py
--rw-rw-rw-   0        0        0     6716 2024-03-27 17:54:16.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/negative_binomial.py
--rw-rw-rw-   0        0        0     6229 2024-03-27 17:54:15.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/poisson.py
--rw-rw-rw-   0        0        0     6427 2024-03-27 17:54:16.000000 phitter-0.0.4/phitter/discrete/discrete_distributions/uniform.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.057476 phitter-0.0.4/phitter/discrete/discrete_measures/
--rw-rw-rw-   0        0        0       50 2024-03-01 00:14:14.000000 phitter-0.0.4/phitter/discrete/discrete_measures/__init__.py
--rw-rw-rw-   0        0        0     3444 2024-03-21 02:11:06.000000 phitter-0.0.4/phitter/discrete/discrete_measures/discrete_measures.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.064407 phitter-0.0.4/phitter/discrete/discrete_statistical_tests/
--rw-rw-rw-   0        0        0      169 2024-02-29 22:46:01.000000 phitter-0.0.4/phitter/discrete/discrete_statistical_tests/__init__.py
--rw-rw-rw-   0        0        0     3249 2024-03-22 02:27:56.000000 phitter-0.0.4/phitter/discrete/discrete_statistical_tests/discrete_test_chi_square.py
--rw-rw-rw-   0        0        0     3012 2024-03-22 02:27:56.000000 phitter-0.0.4/phitter/discrete/discrete_statistical_tests/discrete_test_kolmogorov_smirnov.py
--rw-rw-rw-   0        0        0    18585 2024-03-26 22:00:00.000000 phitter-0.0.4/phitter/discrete/phitter_discrete.py
--rw-rw-rw-   0        0        0    18044 2024-03-26 21:59:59.000000 phitter-0.0.4/phitter/main.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:10:02.068426 phitter-0.0.4/phitter.egg-info/
--rw-rw-rw-   0        0        0    17751 2024-03-29 01:10:01.000000 phitter-0.0.4/phitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5913 2024-03-29 01:10:01.000000 phitter-0.0.4/phitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 01:10:01.000000 phitter-0.0.4/phitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-03-29 01:10:01.000000 phitter-0.0.4/phitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 01:10:01.000000 phitter-0.0.4/phitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2071 2024-03-29 01:09:21.000000 phitter-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 01:10:02.075136 phitter-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.999821 phitter-0.0.5/
+-rw-rw-rw-   0        0        0     1121 2024-03-19 04:53:21.000000 phitter-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    30167 2024-04-20 07:39:05.995295 phitter-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    27138 2024-04-20 07:27:53.000000 phitter-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.554484 phitter-0.0.5/phitter/
+-rw-rw-rw-   0        0        0      114 2024-04-20 07:29:00.000000 phitter-0.0.5/phitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.573203 phitter-0.0.5/phitter/continuous/
+-rw-rw-rw-   0        0        0     5472 2024-03-26 21:53:33.000000 phitter-0.0.5/phitter/continuous/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.915940 phitter-0.0.5/phitter/continuous/continuous_distributions/
+-rw-rw-rw-   0        0        0     5110 2024-03-22 02:27:55.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/__init__.py
+-rw-rw-rw-   0        0        0    11189 2024-04-12 23:05:41.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/alpha.py
+-rw-rw-rw-   0        0        0     8084 2024-04-12 22:33:26.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/arcsine.py
+-rw-rw-rw-   0        0        0     9396 2024-04-13 05:22:33.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/argus.py
+-rw-rw-rw-   0        0        0    12224 2024-04-12 23:05:40.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/beta.py
+-rw-rw-rw-   0        0        0     9762 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/beta_prime.py
+-rw-rw-rw-   0        0        0    10649 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/beta_prime_4p.py
+-rw-rw-rw-   0        0        0     8429 2024-04-12 22:41:08.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/bradford.py
+-rw-rw-rw-   0        0        0     9791 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/burr.py
+-rw-rw-rw-   0        0        0    10094 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/burr_4p.py
+-rw-rw-rw-   0        0        0     7590 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/cauchy.py
+-rw-rw-rw-   0        0        0     6792 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/chi_square.py
+-rw-rw-rw-   0        0        0     8704 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/chi_square_3p.py
+-rw-rw-rw-   0        0        0    10305 2024-04-13 02:28:06.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/dagum.py
+-rw-rw-rw-   0        0        0    10945 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/dagum_4p.py
+-rw-rw-rw-   0        0        0     7701 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/erlang.py
+-rw-rw-rw-   0        0        0     7991 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/erlang_3p.py
+-rw-rw-rw-   0        0        0     6486 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/error_function.py
+-rw-rw-rw-   0        0        0     6620 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/exponential.py
+-rw-rw-rw-   0        0        0     7058 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/exponential_2p.py
+-rw-rw-rw-   0        0        0     7978 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/f.py
+-rw-rw-rw-   0        0        0    10726 2024-04-12 23:05:39.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/f_4p.py
+-rw-rw-rw-   0        0        0     8707 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/fatigue_life.py
+-rw-rw-rw-   0        0        0     8727 2024-04-12 23:01:28.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/folded_normal.py
+-rw-rw-rw-   0        0        0     8244 2024-04-12 23:05:39.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/frechet.py
+-rw-rw-rw-   0        0        0     7919 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/gamma.py
+-rw-rw-rw-   0        0        0     8166 2024-04-12 22:33:13.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/gamma_3p.py
+-rw-rw-rw-   0        0        0     8947 2024-04-12 23:05:41.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_extreme_value.py
+-rw-rw-rw-   0        0        0     9598 2024-04-12 23:05:38.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_gamma.py
+-rw-rw-rw-   0        0        0    10372 2024-04-12 23:05:41.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_gamma_4p.py
+-rw-rw-rw-   0        0        0     9560 2024-04-12 23:05:41.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_logistic.py
+-rw-rw-rw-   0        0        0     7681 2024-04-12 23:05:41.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_normal.py
+-rw-rw-rw-   0        0        0     9924 2024-04-12 23:05:42.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_pareto.py
+-rw-rw-rw-   0        0        0     7441 2024-04-12 23:05:42.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/gibrat.py
+-rw-rw-rw-   0        0        0     7343 2024-04-12 22:33:14.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/gumbel_left.py
+-rw-rw-rw-   0        0        0     7347 2024-04-12 22:33:14.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/gumbel_right.py
+-rw-rw-rw-   0        0        0     6924 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/half_normal.py
+-rw-rw-rw-   0        0        0     6756 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/hyperbolic_secant.py
+-rw-rw-rw-   0        0        0    11466 2024-04-12 23:05:42.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gamma.py
+-rw-rw-rw-   0        0        0    10107 2024-04-12 23:05:43.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gamma_3p.py
+-rw-rw-rw-   0        0        0     6687 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gaussian.py
+-rw-rw-rw-   0        0        0     7732 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gaussian_3p.py
+-rw-rw-rw-   0        0        0     9767 2024-04-12 23:05:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/johnson_sb.py
+-rw-rw-rw-   0        0        0     9407 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/johnson_su.py
+-rw-rw-rw-   0        0        0    10293 2024-04-12 23:01:30.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/kumaraswamy.py
+-rw-rw-rw-   0        0        0     5987 2024-04-12 22:33:16.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/laplace.py
+-rw-rw-rw-   0        0        0     7816 2024-04-12 23:05:43.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/levy.py
+-rw-rw-rw-   0        0        0    10344 2024-04-12 23:01:31.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/loggamma.py
+-rw-rw-rw-   0        0        0     6784 2024-04-12 22:33:23.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/logistic.py
+-rw-rw-rw-   0        0        0    10259 2024-04-12 23:05:44.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/loglogistic.py
+-rw-rw-rw-   0        0        0     9515 2024-04-12 23:05:44.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/loglogistic_3p.py
+-rw-rw-rw-   0        0        0     7260 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/lognormal.py
+-rw-rw-rw-   0        0        0     8561 2024-04-12 23:01:32.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/maxwell.py
+-rw-rw-rw-   0        0        0     8019 2024-04-12 23:01:32.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/moyal.py
+-rw-rw-rw-   0        0        0     7918 2024-04-12 22:33:18.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/nakagami.py
+-rw-rw-rw-   0        0        0     9188 2024-04-12 23:01:32.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_chi_square.py
+-rw-rw-rw-   0        0        0    11602 2024-04-12 23:01:32.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_f.py
+-rw-rw-rw-   0        0        0    12119 2024-04-12 23:01:33.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_t_student.py
+-rw-rw-rw-   0        0        0     6749 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/normal.py
+-rw-rw-rw-   0        0        0    10625 2024-04-12 23:05:44.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/pareto_first_kind.py
+-rw-rw-rw-   0        0        0    10434 2024-04-12 23:05:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/pareto_second_kind.py
+-rw-rw-rw-   0        0        0     9727 2024-04-16 15:58:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/pert.py
+-rw-rw-rw-   0        0        0    10485 2024-04-12 23:01:33.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/power_function.py
+-rw-rw-rw-   0        0        0     7386 2024-04-12 23:05:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/rayleigh.py
+-rw-rw-rw-   0        0        0     7365 2024-04-12 22:33:20.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/reciprocal.py
+-rw-rw-rw-   0        0        0    11142 2024-04-12 23:01:33.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/rice.py
+-rw-rw-rw-   0        0        0     6929 2024-04-12 19:59:29.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/semicircular.py
+-rw-rw-rw-   0        0        0     7222 2024-04-12 22:33:21.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/t_student.py
+-rw-rw-rw-   0        0        0     7734 2024-04-12 23:05:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/t_student_3p.py
+-rw-rw-rw-   0        0        0    10115 2024-04-12 23:01:33.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/trapezoidal.py
+-rw-rw-rw-   0        0        0     9950 2024-04-12 23:05:45.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/triangular.py
+-rw-rw-rw-   0        0        0     6457 2024-04-12 22:33:21.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/uniform.py
+-rw-rw-rw-   0        0        0     8643 2024-04-12 22:33:21.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/weibull.py
+-rw-rw-rw-   0        0        0     9062 2024-04-12 23:01:34.000000 phitter-0.0.5/phitter/continuous/continuous_distributions/weibull_3p.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.921158 phitter-0.0.5/phitter/continuous/continuous_measures/
+-rw-rw-rw-   0        0        0       54 2024-03-01 00:26:16.000000 phitter-0.0.5/phitter/continuous/continuous_measures/__init__.py
+-rw-rw-rw-   0        0        0     5955 2024-04-15 18:54:30.000000 phitter-0.0.5/phitter/continuous/continuous_measures/continuous_measures.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.933598 phitter-0.0.5/phitter/continuous/continuous_statistical_tests/
+-rw-rw-rw-   0        0        0      273 2024-02-29 22:48:49.000000 phitter-0.0.5/phitter/continuous/continuous_statistical_tests/__init__.py
+-rw-rw-rw-   0        0        0     3673 2024-04-12 22:30:39.000000 phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_anderson_darling.py
+-rw-rw-rw-   0        0        0     3352 2024-04-12 22:30:39.000000 phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_chi_square.py
+-rw-rw-rw-   0        0        0     3058 2024-04-12 22:30:39.000000 phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_kolmogorov_smirnov.py
+-rw-rw-rw-   0        0        0    33198 2024-04-20 06:29:58.000000 phitter-0.0.5/phitter/continuous/phitter_continuous.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.940798 phitter-0.0.5/phitter/discrete/
+-rw-rw-rw-   0        0        0      850 2024-03-26 22:02:58.000000 phitter-0.0.5/phitter/discrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.969092 phitter-0.0.5/phitter/discrete/discrete_distributions/
+-rw-rw-rw-   0        0        0      581 2024-03-22 02:27:56.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/__init__.py
+-rw-rw-rw-   0        0        0     6501 2024-04-12 22:33:27.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/bernoulli.py
+-rw-rw-rw-   0        0        0     6886 2024-04-12 22:33:27.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/binomial.py
+-rw-rw-rw-   0        0        0     6547 2024-04-12 22:33:29.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/geometric.py
+-rw-rw-rw-   0        0        0     9068 2024-04-12 23:01:34.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/hypergeometric.py
+-rw-rw-rw-   0        0        0     7582 2024-04-12 22:33:28.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/logarithmic.py
+-rw-rw-rw-   0        0        0     7062 2024-04-12 22:33:28.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/negative_binomial.py
+-rw-rw-rw-   0        0        0     6542 2024-04-12 22:33:29.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/poisson.py
+-rw-rw-rw-   0        0        0     6743 2024-04-12 22:33:28.000000 phitter-0.0.5/phitter/discrete/discrete_distributions/uniform.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.977110 phitter-0.0.5/phitter/discrete/discrete_measures/
+-rw-rw-rw-   0        0        0       50 2024-03-01 00:14:14.000000 phitter-0.0.5/phitter/discrete/discrete_measures/__init__.py
+-rw-rw-rw-   0        0        0     3655 2024-04-15 18:40:05.000000 phitter-0.0.5/phitter/discrete/discrete_measures/discrete_measures.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.987186 phitter-0.0.5/phitter/discrete/discrete_statistical_tests/
+-rw-rw-rw-   0        0        0      169 2024-02-29 22:46:01.000000 phitter-0.0.5/phitter/discrete/discrete_statistical_tests/__init__.py
+-rw-rw-rw-   0        0        0     3247 2024-04-12 22:30:39.000000 phitter-0.0.5/phitter/discrete/discrete_statistical_tests/discrete_test_chi_square.py
+-rw-rw-rw-   0        0        0     3010 2024-04-12 22:30:39.000000 phitter-0.0.5/phitter/discrete/discrete_statistical_tests/discrete_test_kolmogorov_smirnov.py
+-rw-rw-rw-   0        0        0    31748 2024-04-20 06:31:57.000000 phitter-0.0.5/phitter/discrete/phitter_discrete.py
+-rw-rw-rw-   0        0        0    36771 2024-04-19 06:40:06.000000 phitter-0.0.5/phitter/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:39:05.992298 phitter-0.0.5/phitter.egg-info/
+-rw-rw-rw-   0        0        0    30167 2024-04-20 07:39:05.000000 phitter-0.0.5/phitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5913 2024-04-20 07:39:05.000000 phitter-0.0.5/phitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 07:39:05.000000 phitter-0.0.5/phitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-20 07:39:05.000000 phitter-0.0.5/phitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-20 07:39:05.000000 phitter-0.0.5/phitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2118 2024-04-20 07:34:59.000000 phitter-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 07:39:05.999821 phitter-0.0.5/setup.cfg
```

### Comparing `phitter-0.0.4/LICENSE` & `phitter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/phitter/continuous/__init__.py` & `phitter-0.0.5/phitter/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/__init__.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/alpha.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/alpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     https://phitter.io/distributions/continuous/alpha
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the ALPHA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters ALPHA distribution: {"alpha": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/alpha
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -181,15 +182,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "loc": *, "scale": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     alpha, loc, scale = initial_solution
@@ -218,24 +219,24 @@
         #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
         #     eq2 = parametric_median - continuous_measures.median
         #     eq3 = parametric_mode - continuous_measures.mode
 
         #     return (eq1, eq2, eq3)
 
         ## THIS METHOD IS CORRECT, BUT IS VERY SLOW BECAUSE THE INTEGRATION
-        # bnds = ((0, 9, 0), (numpy.inf, continuous_measures.mean, numpy.inf))
+        # bounds = ((0, 9, 0), (numpy.inf, continuous_measures.mean, numpy.inf))
         # x0 = (1, continuous_measures.mean, 1)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"alpha": solution.x[0], "loc": solution.x[1], "scale": solution.x[2]}
 
         # solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
         # parameters = {"alpha": solution[0], "loc": solution[1], "scale": solution[2]}
 
-        scipy_params = scipy.stats.alpha.fit(continuous_measures.data)
+        scipy_params = scipy.stats.alpha.fit(continuous_measures.data_to_fit)
         parameters = {"alpha": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/arcsine.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/arcsine.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/arcsine
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the ARCSINE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters ARCSINE distribution: {"a": *, "b": *}
+        https://phitter.io/distributions/continuous/arcsine
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,15 +167,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *}
         """
         a = continuous_measures.min - 1e-3
         b = continuous_measures.max + 1e-3
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/argus.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/chi_square_3p.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 import numpy
+import scipy.optimize
 import scipy.special
 import scipy.stats
 
 
-class ARGUS:
+class CHI_SQUARE_3P:
     """
-    Argus distribution
-    Parameters ARGUS distribution: {"chi": *, "loc": *, "scale": *}
-    https://phitter.io/distributions/continuous/argus
+    Chi Square distribution
+    Parameters CHI_SQUARE_3P distribution: {"df": *, "loc": *, "scale": *}
+    https://phitter.io/distributions/continuous/chi_square_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the ARGUS distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters ARGUS distribution: {"chi": *, "loc": *, "scale": *}
+        Initializes the CHI_SQUARE_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters CHI_SQUARE_3P distribution: {"df": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/chi_square_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
-        self.chi = self.parameters["chi"]
+        self.df = self.parameters["df"]
         self.loc = self.parameters["loc"]
         self.scale = self.parameters["scale"]
 
     @property
     def name(self):
-        return "argus"
+        return "chi_square_3p"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"chi": 3, "loc": 102, "scale": 0}
+        return {"df": 4, "loc": 10, "scale": 2}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
+        # result, error = scipy.integrate.quad(self.pdf, 0, x)
+        # result = scipy.stats.chi2.cdf(x, self.df, self.loc, self.scale)
         z = lambda t: (t - self.loc) / self.scale
-        # Ψ = lambda t: scipy.stats.norm.cdf(t) - t * scipy.stats.norm.pdf(t)-0.5
-        # print(scipy.stats.argus.cdf(x, self.chi, loc=self.loc, scale=self.scale))
-        # print(1 - Ψ(self.chi * numpy.sqrt(1 - z(x) * z(x))) / Ψ(self.chi))
-        result = 1 - scipy.special.gammainc(1.5, self.chi * self.chi * (1 - z(x) ** 2) / 2) / scipy.special.gammainc(1.5, self.chi * self.chi / 2)
+        result = scipy.special.gammainc(self.df / 2, z(x) / 2)
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
+        # result = scipy.stats.chi2.pdf(x, self.df, loc=self.loc, scale=self.scale)
         z = lambda t: (t - self.loc) / self.scale
-        Ψ = lambda t: scipy.stats.norm.cdf(t) - t * scipy.stats.norm.pdf(t) - 0.5
-        # print(scipy.stats.argus.pdf(x, self.chi, loc=self.loc, scale=self.scale))
-        result = (1 / self.scale) * ((self.chi**3) / (numpy.sqrt(2 * numpy.pi) * Ψ(self.chi))) * z(x) * numpy.sqrt(1 - z(x) * z(x)) * numpy.exp(-0.5 * self.chi**2 * (1 - z(x) * z(x)))
+        result = (1 / self.scale) * (1 / (2 ** (self.df / 2) * scipy.special.gamma(self.df / 2))) * (z(x) ** ((self.df / 2) - 1)) * (numpy.exp(-z(x) / 2))
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        y1 = (1 - u) * scipy.special.gammainc(1.5, (self.chi * self.chi) / 2)
-        y2 = (2 * scipy.special.gammaincinv(1.5, y1)) / (self.chi * self.chi)
-        result = self.loc + self.scale * numpy.sqrt(1 - y2)
+        result = 2 * self.scale * scipy.special.gammaincinv(self.df / 2, u) + self.loc
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -87,117 +85,142 @@
         return None
 
     @property
     def mean(self) -> float:
         """
         Parametric mean
         """
-        return self.loc + self.scale * numpy.sqrt(numpy.pi / 8) * (
-            (self.chi * numpy.exp((-self.chi * self.chi) / 4) * scipy.special.iv(1, (self.chi * self.chi) / 4)) / (scipy.stats.norm.cdf(self.chi) - self.chi * scipy.stats.norm.pdf(self.chi) - 0.5)
-        )
+        return self.df * self.scale + self.loc
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return (
-            self.scale * self.scale * (1 - 3 / (self.chi * self.chi) + (self.chi * scipy.stats.norm.pdf(self.chi)) / (scipy.stats.norm.cdf(self.chi) - self.chi * scipy.stats.norm.pdf(self.chi) - 0.5))
-            - (self.mean - self.loc) ** 2
-        )
+        return self.df * 2 * (self.scale * self.scale)
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
 
     @property
     def skewness(self) -> float:
         """
         Parametric skewness
         """
-        return None
+        return numpy.sqrt(8 / self.df)
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return None
+        return 12 / self.df + 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
 
     @property
     def mode(self) -> float:
         """
         Parametric mode
         """
-        return self.loc + self.scale * (1 / (numpy.sqrt(2) * self.chi)) * numpy.sqrt(self.chi * self.chi - 2 + numpy.sqrt(self.chi * self.chi * self.chi * self.chi + 4))
+        return (self.df - 2) * self.scale + self.loc
 
     @property
     def num_parameters(self) -> int:
         """
         Number of parameters of the distribution
         """
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
-        v1 = self.chi > 0
-        v2 = self.scale > 0
+        v1 = self.df > 0
+        v2 = type(self.df) == int
         return v1 and v2
 
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
-        The parameters are calculated by solving the equations of the measures expected
-        for this distribution.The number of equations to consider is equal to the number
-        of parameters.
+        The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
-        parameters: {"chi": *, "loc": *, "scale": *}
+        parameters: {"df": *, "loc": *, "scale": *}
         """
-        scipy_params = scipy.stats.argus.fit(continuous_measures.data)
-        parameters = {"chi": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
+        # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
+        #     ## Variables declaration
+        #     df, loc, scale = initial_solution
+
+        #     ## Parametric expected expressions
+        #     parametric_mean = df * scale + loc
+        #     parametric_variance = 2 * df * (scale ** 2)
+        #     parametric_skewness = numpy.sqrt(8 / df)
+        #     # parametric_kurtosis = 12 / df  + 3
+
+        #     ## System Equations
+        #     eq1 = parametric_mean - continuous_measures.mean
+        #     eq2 = parametric_variance - continuous_measures.variance
+        #     eq3 = parametric_skewness - continuous_measures.skewness
+        #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
+
+        #     return(eq1, eq2, eq3)
+
+        # solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
+        # print(solution)
+
+        # ## Method 1: Solve system
+        # df = 8 / (continuous_measures.skewness ** 2)
+        # scale = numpy.sqrt(continuous_measures.variance / (2 * df))
+        # loc = continuous_measures.mean - df * scale
+        # parameters = {"df": df, "loc": loc, "scale": scale}
+
+        ## Scipy FIT
+        scipy_params = scipy.stats.chi2.fit(continuous_measures.data_to_fit)
+        parameters = {"df": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
+
         return parameters
 
 
 if __name__ == "__main__":
+    ## Import function to get continuous_measures
     import sys
 
+    import numpy
+
     sys.path.append("../")
     from continuous_measures import CONTINUOUS_MEASURES
 
     ## Import function to get continuous_measures
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_argus.txt"
+    path = "../continuous_distributions_sample/sample_chi_square_3p.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = ARGUS(continuous_measures)
+    distribution = CHI_SQUARE_3P(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/beta.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/beta.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/beta
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BETA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BETA distribution: {"alpha": *, "beta": *, "A": *, "B": *}
+        https://phitter.io/distributions/continuous/beta
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -157,15 +158,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *, "A": *, "B": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -182,25 +183,25 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             eq4 = parametric_kurtosis - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3, eq4)
 
-        bnds = ((0, 0, -numpy.inf, continuous_measures.mean), (numpy.inf, numpy.inf, continuous_measures.mean, numpy.inf))
+        bounds = ((0, 0, -numpy.inf, continuous_measures.mean), (numpy.inf, numpy.inf, continuous_measures.mean, numpy.inf))
         x0 = (1, 1, continuous_measures.min, continuous_measures.max)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"alpha": solution.x[0], "beta": solution.x[1], "A": solution.x[2], "B": solution.x[3]}
 
         v1 = parameters["alpha"] > 0
         v2 = parameters["beta"] > 0
         v3 = parameters["A"] < parameters["B"]
         if (v1 and v2 and v3) == False:
-            scipy_params = scipy.stats.beta.fit(continuous_measures.data)
+            scipy_params = scipy.stats.beta.fit(continuous_measures.data_to_fit)
             parameters = {"alpha": scipy_params[0], "beta": scipy_params[1], "A": scipy_params[2], "B": scipy_params[3]}
         return parameters
 
 
 if __name__ == "__main__":
     ## Import function to get continuous_measures
     import sys
@@ -262,21 +263,21 @@
     # solution = scipy.optimize.fsolve(equations, (1, 1, 1, 1), continuous_measures)
     # parameters = {"alpha": solution[0], "beta": solution[1], "A": solution[2], "B": solution[3]}
     # print(parameters)
     # print("Solve equations time: ", time.time() - ti)
 
     # print("=====")
     # ti = time.time()
-    # scipy_params = scipy.stats.beta.fit(continuous_measures.data)
+    # scipy_params = scipy.stats.beta.fit(continuous_measures.data_to_fit)
     # parameters = {"alpha": scipy_params[0], "beta": scipy_params[1], "A": scipy_params[2], "B": scipy_params[3]}
     # print(parameters)
     # print("Scipy time get parameters: ",time.time() - ti)
 
     # print("=====")
 
     # ti = time.time()
-    # bnds = ((0, 0,  - numpy.inf, continuous_measures.mean), (numpy.inf, numpy.inf, continuous_measures.mean, numpy.inf))
+    # bounds = ((0, 0,  - numpy.inf, continuous_measures.mean), (numpy.inf, numpy.inf, continuous_measures.mean, numpy.inf))
     # x0 = (1, 1, continuous_measures.min, continuous_measures.max)
     # args = ([continuous_measures])
-    # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+    # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
     # print(solution.x)
     # print("Solve equations time: ", time.time() - ti)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/beta_prime.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/beta_prime.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 warnings.filterwarnings("ignore")
 
 
 class BETA_PRIME:
     """
     Beta Prime Distribution
+    Parameters BETA_PRIME distribution: {"alpha": *, "beta": *}
     https://phitter.io/distributions/continuous/beta_prime
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BETA_PRIME distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BETA_PRIME distribution: {"alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/beta_prime
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -171,15 +173,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -200,21 +202,21 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             # eq3 = parametric_skewness - continuous_measures.skewness
             # eq2 = parametric_mode - continuous_measures.mode
 
             return (eq1, eq2)
 
-        scipy_params = scipy.stats.betaprime.fit(continuous_measures.data)
+        scipy_params = scipy.stats.betaprime.fit(continuous_measures.data_to_fit)
 
         try:
-            bnds = ((0, 0), (numpy.inf, numpy.inf))
+            bounds = ((0, 0), (numpy.inf, numpy.inf))
             x0 = (scipy_params[0], scipy_params[1])
             args = [continuous_measures]
-            solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
             parameters = {"alpha": solution.x[0], "beta": solution.x[1]}
         except:
             parameters = {"alpha": scipy_params[0], "beta": scipy_params[1]}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/beta_prime_4p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/beta_prime_4p.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import scipy.stats
 
 warnings.filterwarnings("ignore")
 
 
 class BETA_PRIME_4P:
     """
-    scale Prime 4p Distribution
+    Beta Prime 4P Distribution
+    Parameters BETA_PRIME_4P distribution: {"alpha": *, "beta": *, "loc": *, "scale": *}
     https://phitter.io/distributions/continuous/beta_prime_4p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BETA_PRIME_4P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BETA_PRIME_4P distribution: {"alpha": *, "beta": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/beta_prime_4p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -183,15 +185,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *, "loc": *, "scale": *}
         """
 
         ## In this distribution solve the system is best than scipy estimation.
@@ -209,21 +211,21 @@
             # eq3 = parametric_skewness - continuous_measures.skewness
             eq3 = parametric_median - continuous_measures.median
             eq4 = parametric_mode - continuous_measures.mode
 
             return (eq1, eq2, eq3, eq4)
 
         try:
-            bnds = ((0, 0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+            bounds = ((0, 0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
             x0 = (continuous_measures.mean, continuous_measures.mean, scipy_params[3], continuous_measures.mean)
             args = [continuous_measures]
-            solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
             parameters = {"alpha": solution.x[0], "beta": solution.x[1], "loc": solution.x[3], "scale": solution.x[2]}
         except:
-            scipy_params = scipy.stats.betaprime.fit(continuous_measures.data)
+            scipy_params = scipy.stats.betaprime.fit(continuous_measures.data_to_fit)
             parameters = {"alpha": scipy_params[0], "beta": scipy_params[1], "loc": scipy_params[2], "scale": scipy_params[3]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/bradford.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/bradford.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/bradford
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BRADFORD distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BRADFORD distribution: {"c": *, "min": *, "max": *}
+        https://phitter.io/distributions/continuous/bradford
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -150,15 +151,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"c": *, "min": *, "max": *}
         """
 
         _min = continuous_measures.min - 1e-3
@@ -173,17 +174,15 @@
 
             ## System Equations
             eq1 = parametric_mean - continuous_measures.mean
 
             return eq1
 
         solution = scipy.optimize.fsolve(equations, (1), continuous_measures)
-
         parameters = {"c": solution[0], "min": _min, "max": _max}
-
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/burr.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/burr.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     https://phitter.io/distributions/continuous/burr
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BURR distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BURR distribution: {"A": *, "B": *, "C": *}
+        https://phitter.io/distributions/continuous/burr
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -175,15 +176,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"A": *, "B": *, "C": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     ## Variables declaration
@@ -208,20 +209,20 @@
         #     # eq3 = parametric_skewness - continuous_measures.skewness
         #     # eq2 = parametric_variance - continuous_measures.variance
 
         #     return (eq1, eq2, eq3)
 
         ## Solve equations system
         # x0 = [continuous_measures.mean, continuous_measures.mean, continuous_measures.mean]
-        # b = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = b, args=([continuous_measures]))
+        # bounds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = b, args=([continuous_measures]))
         # parameters = {"A": solution.x[0], "B": solution.x[1], "C": solution.x[2]}
 
         # Scipy class
-        scipy_params = scipy.stats.burr12.fit(continuous_measures.data)
+        scipy_params = scipy.stats.burr12.fit(continuous_measures.data_to_fit)
         parameters = {"A": scipy_params[3], "B": scipy_params[0], "C": scipy_params[1]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/burr_4p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/burr_4p.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     https://phitter.io/distributions/continuous/burr_4p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the BURR_4P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters BURR_4P distribution: {"A": *, "B": *, "C": *, "loc": *}
+        https://phitter.io/distributions/continuous/burr_4p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -176,15 +177,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"A": *, "B": *, "C": *, "loc": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     ## Variables declaration
@@ -207,21 +208,21 @@
         #     eq3 = parametric_kurtosis - continuous_measures.kurtosis
         #     eq4 = parametric_mode - continuous_measures.mode
 
         #     return (eq1, eq2, eq3, eq4)
 
         # ## Solve equations system
         # x0 = [continuous_measures.mean, continuous_measures.mean, continuous_measures.mean, continuous_measures.mean]
-        # b = ((1e-5, 1e-5, 1e-5,  - numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = b, args=([continuous_measures]))
+        # bounds = ((1e-5, 1e-5, 1e-5,  - numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = b, args=([continuous_measures]))
         # parameters = {"A": solution.x[0], "B": solution.x[1], "C": solution.x[2], "loc": solution.x[3]}
         # print(parameters)
 
         ## Scipy class
-        scipy_params = scipy.stats.burr12.fit(continuous_measures.data)
+        scipy_params = scipy.stats.burr12.fit(continuous_measures.data_to_fit)
         parameters = {"A": scipy_params[3], "B": scipy_params[0], "C": scipy_params[1], "loc": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     ## Import function to get continuous_measures
     import sys
@@ -235,15 +236,15 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_burr_4P.txt"
+    path = "../continuous_distributions_sample/sample_burr_4p.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
     distribution = BURR_4P(continuous_measures)
     print(distribution.get_parameters(continuous_measures))
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/cauchy.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/cauchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/cauchy
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the CAUCHY distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters CAUCHY distribution: {"x0": *, "gamma": *}
+        https://phitter.io/distributions/continuous/cauchy
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -141,15 +142,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"x0": *, "gamma": *}
         """
         # ## First estimation
         # x0_ini = continuous_measures.median
@@ -160,15 +161,15 @@
         # ## Maximum Likelihood Estimation Cauchy distribution
         # def objective(x):
         #     x0, gamma = x
         #     return - sum([numpy.log(1 / (numpy.pi * gamma * (1 + ((d - x0) / gamma) ** 2))) for d in continuous_measures.data])
         # solution = scipy.optimize.minimize(objective, [x0_ini, gamma_ini], method="SLSQP", bounds = [(-numpy.inf, numpy.inf),(0,numpy.inf)])
         # print(solution)
 
-        scipy_params = scipy.stats.cauchy.fit(continuous_measures.data)
+        scipy_params = scipy.stats.cauchy.fit(continuous_measures.data_to_fit)
 
         ## Results
         parameters = {"x0": scipy_params[0], "gamma": scipy_params[1]}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/chi_square.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/chi_square.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/chi_square
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the CHI_SQUARE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters CHI_SQUARE distribution: {"df": *}
+        https://phitter.io/distributions/continuous/chi_square
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -147,15 +148,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"df": *}
         """
         parameters = {"df": round(continuous_measures.mean)}
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/chi_square_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gaussian_3p.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 import numpy
-import scipy.optimize
-import scipy.special
 import scipy.stats
 
 
-class CHI_SQUARE_3P:
+class INVERSE_GAUSSIAN_3P:
     """
-    Chi Square distribution
-    Parameters CHI_SQUARE_3P distribution: {"df": *, "loc": *, "scale": *}
-    https://phitter.io/distributions/continuous/chi_square_3p
+    Inverse Gaussian distribution
+    Also known like Wald distribution
+    Parameters INVERSE_GAUSSIAN_3P distribution: {"mu": *, "lambda": *, "loc": *}
+    https://phitter.io/distributions/continuous/inverse_gaussian_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the CHI_SQUARE_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters CHI_SQUARE_3P distribution: {"df": *, "loc": *, "scale": *}
+        Initializes the INVERSE_GAUSSIAN_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters INVERSE_GAUSSIAN_3P distribution: {"mu": *, "lambda": *, "loc": *}
+        https://phitter.io/distributions/continuous/inverse_gaussian_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
-        self.df = self.parameters["df"]
+        self.mu = self.parameters["mu"]
+        self.lambda_ = self.parameters["lambda"]
         self.loc = self.parameters["loc"]
-        self.scale = self.parameters["scale"]
 
     @property
     def name(self):
-        return "chi_square_3p"
+        return "inverse_gaussian_3p"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"df": 4, "loc": 10, "scale": 2}
+        return {"mu": 9, "lambda": 77, "loc": 60}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        # result, error = scipy.integrate.quad(self.pdf, 0, x)
-        # result = scipy.stats.chi2.cdf(x, self.df, self.loc, self.scale)
-        z = lambda t: (t - self.loc) / self.scale
-        result = scipy.special.gammainc(self.df / 2, z(x) / 2)
+        # result = scipy.stats.norm.cdf(numpy.sqrt(self.lambda_ / (x - self.loc)) * (((x - self.loc) / self.mu) - 1)) + numpy.exp(2 * self.lambda_ / self.mu) * scipy.stats.norm.cdf(-numpy.sqrt(self.lambda_ / (x - self.loc)) * (((x - self.loc) / self.mu) + 1))
+        result = scipy.stats.invgauss.cdf(x, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        # result = scipy.stats.chi2.pdf(x, self.df, loc=self.loc, scale=self.scale)
-        z = lambda t: (t - self.loc) / self.scale
-        result = (1 / self.scale) * (1 / (2 ** (self.df / 2) * scipy.special.gamma(self.df / 2))) * (z(x) ** ((self.df / 2) - 1)) * (numpy.exp(-z(x) / 2))
+        # result = numpy.sqrt(self.lambda_ / (2 * numpy.pi * (x - self.loc) ** 3)) * numpy.exp(-(self.lambda_ * ((x - self.loc) - self.mu) ** 2) / (2 * self.mu**2 * (x - self.loc)))
+        result = scipy.stats.invgauss.pdf(x, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = 2 * self.scale * scipy.special.gammaincinv(self.df / 2, u) + self.loc
+        result = scipy.stats.invgauss.ppf(u, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -84,142 +81,113 @@
         return None
 
     @property
     def mean(self) -> float:
         """
         Parametric mean
         """
-        return self.df * self.scale + self.loc
+        return self.mu + self.loc
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return self.df * 2 * (self.scale * self.scale)
+        return self.mu**3 / self.lambda_
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
 
     @property
     def skewness(self) -> float:
         """
         Parametric skewness
         """
-        return numpy.sqrt(8 / self.df)
+        return 3 * numpy.sqrt(self.mu / self.lambda_)
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 12 / self.df + 3
+        return 15 * (self.mu / self.lambda_) + 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
 
     @property
     def mode(self) -> float:
         """
         Parametric mode
         """
-        return (self.df - 2) * self.scale + self.loc
+        return self.loc + self.mu * (numpy.sqrt(1 + (9 * self.mu * self.mu) / (4 * self.lambda_ * self.lambda_)) - (3 * self.mu) / (2 * self.lambda_))
 
     @property
     def num_parameters(self) -> int:
         """
         Number of parameters of the distribution
         """
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
-        v1 = self.df > 0
-        v2 = type(self.df) == int
+        v1 = self.mu > 0
+        v2 = self.lambda_ > 0
         return v1 and v2
 
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
-        continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+        continuous_measures : dict
+            {"mu": * , "variance": * , "skewness": * , "kurtosis": * , "data": * }
 
         Returns
         =======
-        parameters: {"df": *, "loc": *, "scale": *}
+        parameters: {"mu": *, "lambda": *, "loc": *}
         """
-        # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
-        #     ## Variables declaration
-        #     df, loc, scale = initial_solution
-
-        #     ## Parametric expected expressions
-        #     parametric_mean = df * scale + loc
-        #     parametric_variance = 2 * df * (scale ** 2)
-        #     parametric_skewness = numpy.sqrt(8 / df)
-        #     # parametric_kurtosis = 12 / df  + 3
-
-        #     ## System Equations
-        #     eq1 = parametric_mean - continuous_measures.mean
-        #     eq2 = parametric_variance - continuous_measures.variance
-        #     eq3 = parametric_skewness - continuous_measures.skewness
-        #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
-
-        #     return(eq1, eq2, eq3)
-
-        # solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
-        # print(solution)
-
-        # ## Method 1: Solve system
-        # df = 8 / (continuous_measures.skewness ** 2)
-        # scale = numpy.sqrt(continuous_measures.variance / (2 * df))
-        # loc = continuous_measures.mean - df * scale
-        # parameters = {"df": df, "loc": loc, "scale": scale}
-
-        ## Scipy FIT
-        scipy_params = scipy.stats.chi2.fit(continuous_measures.data)
-        parameters = {"df": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
+        mu = 3 * numpy.sqrt(continuous_measures.variance / (continuous_measures.skewness**2))
+        lambda_ = mu**3 / continuous_measures.variance
+        loc = continuous_measures.mean - mu
 
+        parameters = {"mu": mu, "lambda": lambda_, "loc": loc}
         return parameters
 
 
 if __name__ == "__main__":
-    ## Import function to get continuous_measures
     import sys
 
-    import numpy
-
     sys.path.append("../")
     from continuous_measures import CONTINUOUS_MEASURES
 
     ## Import function to get continuous_measures
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_chi_square_3p.txt"
+    path = "../continuous_distributions_sample/sample_inverse_gaussian_3p.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = CHI_SQUARE_3P(continuous_measures)
+    distribution = INVERSE_GAUSSIAN_3P(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/dagum.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/dagum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import numpy
 import scipy.optimize
 import scipy.special
+import scipy.stats
 
 
 class DAGUM:
     """
     Dagum distribution
     Parameters DAGUM distribution: {"a": *, "b": *, "p": *}
     https://phitter.io/distributions/continuous/dagum
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the DAGUM distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters DAGUM distribution: {"a": *, "b": *, "p": *}
+        https://phitter.io/distributions/continuous/dagum
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -167,37 +169,27 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *, "p": *}
         """
 
         def sse(parameters: dict) -> float:
             def __pdf(x: float, params: dict) -> float:
                 return (params["a"] * params["p"] / x) * (((x / params["b"]) ** (params["a"] * params["p"])) / ((((x / params["b"]) ** (params["a"])) + 1) ** (params["p"] + 1)))
 
-            ## Frequencies of histogram
-            frequencies, bin_edges = numpy.histogram(continuous_measures.data, density=True)
-
-            ## Central values of histogram
-            central_values = [(bin_edges[i] + bin_edges[i + 1]) / 2 for i in range(len(bin_edges) - 1)]
-
-            ## Calculate fitted PDF and error with fit in distribution
-            pdf_values = [__pdf(c, parameters) for c in central_values]
-
-            ## Calculate SSE (sum of squared estimate of errors)
-            sse = numpy.sum(numpy.power(frequencies - pdf_values, 2))
-
+            pdf_values = __pdf(continuous_measures.central_values, parameters)
+            sse = numpy.sum(numpy.power(continuous_measures.densities_frequencies - pdf_values, 2))
             return sse
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
             ## Variables declaration
             a, b, p = initial_solution
 
             ## Generatred moments function (not - centered)
@@ -211,28 +203,29 @@
             # parametric_median = b * ((2 ** (1 / p)) - 1) ** (-1 / a)
             parametric_mode = b * ((a * p - 1) / (a + 1)) ** (1 / a)
 
             ## System Equations
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_mode - continuous_measures.mode
-            # eq3 = parametric_median - continuous_measures.median
+            # eq2 = parametric_median - continuous_measures.median
 
             return (eq1, eq2, eq3)
 
         ## Scipy Burr3 = Dagum parameter
-        s0_burr3_sc = scipy.stats.burr.fit(continuous_measures.data)
+        s0_burr3_sc = scipy.stats.burr.fit(continuous_measures.data_to_fit)
+
         parameters_sc = {"a": s0_burr3_sc[0], "b": s0_burr3_sc[3], "p": s0_burr3_sc[1]}
 
         ##  Least Square Method
         a0 = s0_burr3_sc[0]
         b0 = s0_burr3_sc[3]
         x0 = [a0, b0, 1]
-        b = ((1e-5, 1e-5, 1e-5), (numpy.inf, numpy.inf, numpy.inf))
-        solution = scipy.optimize.least_squares(equations, x0, bounds=b, args=([continuous_measures]))
+        bounds = ((1e-5, 1e-5, 1e-5), (numpy.inf, numpy.inf, numpy.inf))
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures]))
         parameters_ls = {"a": solution.x[0], "b": solution.x[1], "p": solution.x[2]}
 
         sse_sc = sse(parameters_sc)
         sse_ls = sse(parameters_ls)
 
         if a0 <= 2:
             return parameters_sc
@@ -258,14 +251,17 @@
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
     path = "../continuous_distributions_sample/sample_dagum.txt"
     data = get_data(path)
+
+    data = DAGUM(init_parameters_examples=True).sample(10000000)
+
     continuous_measures = CONTINUOUS_MEASURES(data)
     distribution = DAGUM(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/dagum_4p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/dagum_4p.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     https://phitter.io/distributions/continuous/dagum_4p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the DAGUM_4P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters DAGUM_4P distribution: {"a": *, "b": *, "p": *, "loc": *}
+        https://phitter.io/distributions/continuous/dagum_4p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -172,15 +173,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *, "p": *, "loc": *}
         """
 
         def sse(parameters: dict) -> float:
@@ -223,24 +224,24 @@
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_median - continuous_measures.median
             eq4 = parametric_mode - continuous_measures.mode
 
             return (eq1, eq2, eq3, eq4)
 
         ## Scipy Burr3 = Dagum parameter
-        s0_burr3_sc = scipy.stats.burr.fit(continuous_measures.data)
+        s0_burr3_sc = scipy.stats.burr.fit(continuous_measures.data_to_fit)
         parameters_sc = {"a": s0_burr3_sc[0], "b": s0_burr3_sc[3], "p": s0_burr3_sc[1], "loc": s0_burr3_sc[2]}
 
         if s0_burr3_sc[0] <= 2:
             return parameters_sc
         else:
             a0 = s0_burr3_sc[0]
             x0 = [a0, 1, 1, continuous_measures.mean]
-            b = ((1e-5, 1e-5, 1e-5, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
-            solution = scipy.optimize.least_squares(equations, x0, bounds=b, args=([continuous_measures]))
+            bounds = ((1e-5, 1e-5, 1e-5, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures]))
             parameters_ls = {"a": solution.x[0], "b": solution.x[1], "p": solution.x[2], "loc": solution.x[3]}
 
             sse_sc = sse(parameters_sc)
             sse_ls = sse(parameters_ls)
 
             if sse_sc < sse_ls:
                 return parameters_sc
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/erlang.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/erlang.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/erlang
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the ERLANG distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters ERLANG distribution: {"k": *, "beta": *}
+        https://phitter.io/distributions/continuous/erlang
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,15 +167,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"k": *, "beta": *}
         """
         k = round(continuous_measures.mean**2 / continuous_measures.variance)
         beta = continuous_measures.variance / continuous_measures.mean
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/erlang_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/erlang_3p.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/erlang_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the ERLANG_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters ERLANG_3P distribution: {"k": *, "beta": *, "loc": *}
+        https://phitter.io/distributions/continuous/erlang_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,15 +167,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"k": *, "beta": *, "loc": *}
         """
         k = round((2 / continuous_measures.skewness) ** 2)
         beta = numpy.sqrt(continuous_measures.variance / ((2 / continuous_measures.skewness) ** 2))
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/error_function.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/error_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/error_function
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the ERROR_FUNCTION distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters ERROR_FUNCTION distribution: {"h": *}
+        https://phitter.io/distributions/continuous/error_function
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -139,15 +140,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"h": *}
         """
         h = numpy.sqrt(1 / (2 * continuous_measures.variance))
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/exponential.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/exponential.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     https://phitter.io/distributions/continuous/exponential
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the EXPONENTIAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters EXPONENTIAL distribution: {"lambda": *}
+        https://phitter.io/distributions/continuous/exponential
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -141,15 +142,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *}
         """
         lambda_ = 1 / continuous_measures.mean
         parameters = {"lambda": lambda_}
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/exponential_2p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/exponential_2p.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     https://phitter.io/distributions/continuous/exponential_2p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the EXPONENTIAL_2P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters EXPONENTIAL_2P distribution: {"lambda": *, "loc": *}
+        https://phitter.io/distributions/continuous/exponential_2p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -142,15 +143,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *, "loc": *}
         """
         ## Method: Solve system
         lambda_ = (1 - numpy.log(2)) / (continuous_measures.mean - continuous_measures.median)
@@ -170,15 +171,15 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_exponential_2P.txt"
+    path = "../continuous_distributions_sample/sample_exponential_2p.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
     distribution = EXPONENTIAL_2P(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.get_parameters(continuous_measures)}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/f.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/f.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/f
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the F distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters F distribution: {"df1": *, "df2": *}
+        https://phitter.io/distributions/continuous/f
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,22 +167,22 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"df1": *, "df2": *}
         """
         ## Scipy parameters of distribution
-        scipy_params = scipy.stats.f.fit(continuous_measures.data)
+        scipy_params = scipy.stats.f.fit(continuous_measures.data_to_fit)
 
         ## Results
         parameters = {"df1": scipy_params[0], "df2": scipy_params[1]}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/f_4p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/f_4p.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/f_4p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the F_4P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters F_4P distribution: {"df1": *, "df2": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/f_4p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -177,15 +178,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"df1": *, "df2": *, "loc": *, "scale": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -210,22 +211,22 @@
             # eq2 = parametric_skewness - continuous_measures.skewness
             # eq2 = parametric_kurtosis  - continuous_measures.kurtosis
             eq3 = parametric_median - continuous_measures.median
             eq4 = parametric_mode - continuous_measures.mode
             return (eq1, eq2, eq3, eq4)
 
         try:
-            bnds = ((0, 0, -numpy.inf, 0), (numpy.inf, numpy.inf, continuous_measures.min, numpy.inf))
+            bounds = ((0, 0, -numpy.inf, 0), (numpy.inf, numpy.inf, continuous_measures.min, numpy.inf))
             x0 = (1, continuous_measures.standard_deviation, continuous_measures.min, continuous_measures.standard_deviation)
             args = [continuous_measures]
-            solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
             parameters = {"df1": solution.x[0], "df2": solution.x[1], "loc": solution.x[2], "scale": solution.x[3]}
         except:
             ## Scipy parameters of distribution
-            scipy_params = scipy.stats.f.fit(continuous_measures.data)
+            scipy_params = scipy.stats.f.fit(continuous_measures.data_to_fit)
 
             ## Results
             parameters = {"df1": scipy_params[0], "df2": scipy_params[1], "loc": scipy_params[2], "scale": scipy_params[3]}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/fatigue_life.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/fatigue_life.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/fatigue_life
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the FATIGUE_LIFE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters FATIGUE_LIFE distribution: {"gamma": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/fatigue_life
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -150,15 +151,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"gamma": *, "loc": *, "scale": *}
         """
         ## NO SE ESTÁN RESOLVIENDO LAS ECUACIONES PARA GAMMA = 5, scale = 10, loc = 5
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -175,15 +176,15 @@
         #     eq2 = parametric_variance - continuous_measures.variance
         #     eq3 = parametric_skewness - continuous_measures.skewness
 
         #     return (eq1, eq2, eq3)
 
         # solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
         # print(solution)
-        scipy_params = scipy.stats.fatiguelife.fit(continuous_measures.data)
+        scipy_params = scipy.stats.fatiguelife.fit(continuous_measures.data_to_fit)
         parameters = {"gamma": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/folded_normal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/folded_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/folded_normal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the FOLDED_NORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters FOLDED_NORMAL distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/folded_normal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -186,16 +187,16 @@
             # System Equations
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
 
             return (eq1, eq2)
 
         x0 = [continuous_measures.mean, continuous_measures.standard_deviation]
-        b = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
-        solution = scipy.optimize.least_squares(equations, x0, bounds=b, args=([continuous_measures]))
+        bounds = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures]))
         parameters = {"mu": solution.x[0], "sigma": solution.x[1]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/frechet.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/frechet.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/frechet
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the FRECHET distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters FRECHET distribution: {"alpha": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/frechet
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -172,21 +173,21 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "loc": *, "scale": *}
         """
-        scipy_params = scipy.stats.invweibull.fit(continuous_measures.data)
+        scipy_params = scipy.stats.invweibull.fit(continuous_measures.data_to_fit)
         parameters = {"alpha": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/gamma.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/gamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/gamma
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GAMMA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GAMMA distribution: {"alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/gamma
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -169,15 +170,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *}
         """
         alpha = continuous_measures.mean**2 / continuous_measures.variance
         beta = continuous_measures.variance / continuous_measures.mean
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/gamma_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/gamma_3p.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/gamma_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GAMMA_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GAMMA_3P distribution: {"alpha": *, "loc": *, "beta": *}
+        https://phitter.io/distributions/continuous/gamma_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -170,15 +171,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "loc": *, "beta": *}
         """
         alpha = (2 / continuous_measures.skewness) ** 2
         beta = numpy.sqrt(continuous_measures.variance / alpha)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_extreme_value.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_extreme_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/generalized_extreme_value
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_EXTREME_VALUE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_EXTREME_VALUE distribution: {"xi": *, "mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/generalized_extreme_value
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -189,21 +190,21 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"xi": *, "mu": *, "sigma": *}
         """
-        scipy_params = scipy.stats.genextreme.fit(continuous_measures.data)
+        scipy_params = scipy.stats.genextreme.fit(continuous_measures.data_to_fit)
         parameters = {"xi": -scipy_params[0], "mu": scipy_params[1], "sigma": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_gamma.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_gamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     https://phitter.io/distributions/continuous/generalized_gamma
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_GAMMA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_GAMMA distribution: {"a": *, "d": *, "p": *}
+        https://phitter.io/distributions/continuous/generalized_gamma
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -170,15 +171,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "d": *, "p": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -201,22 +202,22 @@
 
         try:
             ## scipy.optimize.fsolve is 100x faster than least square but sometimes return solutions < 0
             solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
 
             ## If return a perameter < 0 then use least_square with restriction
             if all(x > 0 for x in solution) is False or all(x == 1 for x in solution) is True:
-                bnds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
+                bounds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
                 x0 = (1, 1, 1)
                 args = [continuous_measures]
-                response = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+                response = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
                 solution = response.x
             parameters = {"a": solution[0], "d": solution[1], "p": solution[2]}
         except:
-            scipy_params = scipy.stats.gengamma.fit(continuous_measures.data)
+            scipy_params = scipy.stats.gengamma.fit(continuous_measures.data_to_fit)
             parameters = {"a": scipy_params[0], "c": scipy_params[1], "mu": scipy_params[2]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_gamma_4p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_gamma_4p.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/generalized_gamma_4p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_GAMMA_4P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_GAMMA_4P distribution: {"a": *, "d": *, "p": *, "loc": *}
+        https://phitter.io/distributions/continuous/generalized_gamma_4p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,15 +167,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "d": *, "p": *, "loc": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -200,23 +201,23 @@
 
         ## scipy.optimize.fsolve is 100x faster than least square but sometimes return solutions < 0
         solution = scipy.optimize.fsolve(equations, (1, 1, 1, 1), continuous_measures)
 
         ## If return a perameter < 0 then use least_square with restriction
         if all(x > 0 for x in solution) is False or all(x == 1 for x in solution) is True:
             try:
-                bnds = ((0, 0, 0, 0), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+                bounds = ((0, 0, 0, 0), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
                 if continuous_measures.mean < 0:
-                    bnds = ((0, 0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, 0))
+                    bounds = ((0, 0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf, 0))
                 x0 = (1, 1, 1, continuous_measures.mean)
                 args = [continuous_measures]
-                response = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+                response = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
                 solution = response.x
             except:
-                scipy_params = scipy.stats.gengamma.fit(continuous_measures.data)
+                scipy_params = scipy.stats.gengamma.fit(continuous_measures.data_to_fit)
                 solution = [scipy_params[3], scipy_params[0], scipy_params[1], scipy_params[2]]
 
         parameters = {"a": solution[0], "d": solution[1], "p": solution[2], "loc": solution[3]}
 
         return parameters
 
 
@@ -249,10 +250,10 @@
     print(f"mean: {distribution.mean} - {continuous_measures.mean}")
     print(f"variance: {distribution.variance} - {continuous_measures.variance}")
     print(f"skewness: {distribution.skewness} - {continuous_measures.skewness}")
     print(f"kurtosis: {distribution.kurtosis} - {continuous_measures.kurtosis}")
     print(f"median: {distribution.median} - {continuous_measures.median}")
     print(f"mode: {distribution.mode} - {continuous_measures.mode}")
 
-    scipy_params = scipy.stats.gengamma.fit(continuous_measures.data)
+    scipy_params = scipy.stats.gengamma.fit(continuous_measures.data_to_fit)
     parameters = {"a": scipy_params[3], "d": scipy_params[0], "p": scipy_params[1], "loc": scipy_params[2]}
     print(parameters)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_logistic.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/generalized_logistic
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_LOGISTIC distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_LOGISTIC distribution: {"loc": *, "scale": *, "c": *}
+        https://phitter.io/distributions/continuous/generalized_logistic
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -148,15 +149,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"loc": *, "scale": *, "c": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -184,20 +185,20 @@
         # ## scipy.optimize.fsolve methods
         # solution = scipy.optimize.fsolve(equations, (1, 1, 1), continuous_measures)
         # parameters = {"loc": solution[0], "scale": solution[1], "c": solution[2]}
         # print(parameters)
 
         ## least square methods
         x0 = [continuous_measures.mean, continuous_measures.mean, continuous_measures.mean]
-        b = ((1e-5, -numpy.inf, 1e-5), (numpy.inf, numpy.inf, numpy.inf))
-        solution = scipy.optimize.least_squares(equations, x0, bounds=b, args=([continuous_measures]))
+        bounds = ((1e-5, -numpy.inf, 1e-5), (numpy.inf, numpy.inf, numpy.inf))
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures]))
         parameters = {"c": solution.x[0], "loc": solution.x[1], "scale": solution.x[2]}
 
         # ## scipy methods
-        # scipy_params = scipy.stats.genlogistic.fit(continuous_measures.data)
+        # scipy_params = scipy.stats.genlogistic.fit(continuous_measures.data_to_fit)
         # parameters = {"loc": scipy_params[1], "scale": scipy_params[2], "c": scipy_params[0]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_normal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     * Subbotin distribution
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_NORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_NORMAL distribution: {"beta": *, "mu": *, "alpha": *}
+        https://phitter.io/distributions/continuous/generalized_normal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -150,21 +151,21 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"beta": *, "mu": *, "alpha": *}
         """
-        scipy_params = scipy.stats.gennorm.fit(continuous_measures.data)
+        scipy_params = scipy.stats.gennorm.fit(continuous_measures.data_to_fit)
         parameters = {"beta": scipy_params[0], "mu": scipy_params[1], "alpha": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/generalized_pareto.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/generalized_pareto.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/generalized_pareto
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GENERALIZED_PARETO distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GENERALIZED_PARETO distribution: {"c": *, "mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/generalized_pareto
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -149,15 +150,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"c": *, "mu": *, "sigma": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -182,23 +183,23 @@
 
             return (eq1, eq2, eq3)
 
         ## The scipy genpareto.fit is good from samples whit c > 0
         ## but it's not so much when c < 0.
         ## The solution of system of equation is so good. The problem is that
         ## the continuous_measures of genpareto distributions is not defined from c >  1 / 4 (kurtosis)
-        scipy_params = scipy.stats.genpareto.fit(continuous_measures.data)
+        scipy_params = scipy.stats.genpareto.fit(continuous_measures.data_to_fit)
         parameters = {"c": scipy_params[0], "mu": scipy_params[1], "sigma": scipy_params[2]}
 
         if parameters["c"] < 0:
-            scipy_params = scipy.stats.genpareto.fit(continuous_measures.data)
+            scipy_params = scipy.stats.genpareto.fit(continuous_measures.data_to_fit)
             c0 = scipy_params[0]
             x0 = [c0, continuous_measures.min, 1]
-            b = ((-numpy.inf, -numpy.inf, 0), (numpy.inf, continuous_measures.min, numpy.inf))
-            solution = scipy.optimize.least_squares(equations, x0, bounds=b, args=([continuous_measures]))
+            bounds = ((-numpy.inf, -numpy.inf, 0), (numpy.inf, continuous_measures.min, numpy.inf))
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures]))
             parameters = {"c": solution.x[0], "mu": solution.x[1], "sigma": solution.x[2]}
 
             ## When c < 0 the domain of of x is [mu, mu - sigma / c]
             ## Forthis reason mu < continuous_measures.min and mu - sigma / c < continuous_measures.max
             parameters["mu"] = min(parameters["mu"], continuous_measures.min - 1e-3)
             delta_sigma = parameters["c"] * (parameters["mu"] - continuous_measures.max) - parameters["sigma"]
             parameters["sigma"] = parameters["sigma"] + delta_sigma + 1e-8
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/gibrat.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/gibrat.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/gibrat
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GIBRAT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GIBRAT distribution: {"loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/gibrat
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -149,23 +150,23 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"loc": *, "scale": *}
         """
         # loc = continuous_measures.min - 1e-3
         # scale = (continuous_measures.mean - loc) / numpy.sqrt(numpy.e)
-        scipy_params = scipy.stats.gibrat.fit(continuous_measures.data)
+        scipy_params = scipy.stats.gibrat.fit(continuous_measures.data_to_fit)
         parameters = {"loc": scipy_params[0], "scale": scipy_params[1]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/gumbel_left.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/gumbel_left.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/gumbel_left
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GUMBEL_LEFT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GUMBEL_LEFT distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/gumbel_left
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -143,15 +144,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"mu": *, "sigma": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/gumbel_right.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/gumbel_right.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/gumbel_right
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the GUMBEL_RIGHT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters GUMBEL_RIGHT distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/gumbel_right
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -144,15 +145,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"mu": *, "sigma": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/half_normal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/half_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/half_normal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the HALF_NORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters HALF_NORMAL distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/half_normal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/hyperbolic_secant.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/hyperbolic_secant.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     https://phitter.io/distributions/continuous/hyperbolic_secant
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the HYPERBOLIC_SECANT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters HYPERBOLIC_SECANT distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/hyperbolic_secant
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gamma.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gamma.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     https://phitter.io/distributions/continuous/inverse_gamma
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the INVERSE_GAMMA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters INVERSE_GAMMA distribution: {"alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/inverse_gamma
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -176,15 +177,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     ## Variables declaration
@@ -203,21 +204,21 @@
         #     eq1 = parametric_mean - continuous_measures.mean
         #     eq2 = parametric_variance - continuous_measures.variance
         #     # eq3 = parametric_skewness - continuous_measures.skewness
         #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
         #     return (eq1, eq2)
 
-        # bnds = ((0, 0), (numpy.inf, numpy.inf))
+        # bounds = ((0, 0), (numpy.inf, numpy.inf))
         # x0 = (5, 1)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"alpha": solution.x[0], "beta": solution.x[1]}
 
-        scipy_params = scipy.stats.invgamma.fit(continuous_measures.data)
+        scipy_params = scipy.stats.invgamma.fit(continuous_measures.data_to_fit)
         parameters = {"alpha": scipy_params[0], "beta": scipy_params[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
@@ -273,20 +274,20 @@
     #     eq2 = parametric_variance - continuous_measures.variance
     #     # eq3 = parametric_skewness - continuous_measures.skewness
     #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
     #     return (eq1, eq2)
 
     # ti = time.time()
-    # bnds = ((0, 0), (numpy.inf, numpy.inf))
+    # bounds = ((0, 0), (numpy.inf, numpy.inf))
     # x0 = (1.1, 1)
     # args = [continuous_measures]
-    # solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+    # solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
     # parameters = {"alpha": solution.x[0], "beta": solution.x[1]}
     # print(parameters)
     # print("Solve equations time: ", time.time() - ti)
 
     # ti = time.time()
-    # scipy_params = scipy.stats.invgamma.fit(continuous_measures.data)
+    # scipy_params = scipy.stats.invgamma.fit(continuous_measures.data_to_fit)
     # parameters = {"alpha": scipy_params[0], "beta": scipy_params[2]}
     # print(parameters)
     # print("Scipy time get parameters: ", time.time() - ti)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gamma_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gamma_3p.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     https://phitter.io/distributions/continuous/inverse_gamma_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the INVERSE_GAMMA_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters INVERSE_GAMMA_3P distribution: {"alpha": *, "beta": *, "loc": *}
+        https://phitter.io/distributions/continuous/inverse_gamma_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -177,15 +178,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *, "loc": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -206,21 +207,21 @@
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3)
 
         try:
-            bnds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+            bounds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
             x0 = (2, 1, continuous_measures.mean)
             args = [continuous_measures]
-            solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+            solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
             parameters = {"alpha": solution.x[0], "beta": solution.x[1], "loc": solution.x[2]}
         except:
-            scipy_params = scipy.stats.invgamma.fit(continuous_measures.data)
+            scipy_params = scipy.stats.invgamma.fit(continuous_measures.data_to_fit)
             parameters = {"alpha": scipy_params[0], "loc": scipy_params[1], "beta": scipy_params[2]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gaussian.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/inverse_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/inverse_gaussian
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the INVERSE_GAUSSIAN distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters INVERSE_GAUSSIAN distribution: {"mu": *, "lambda": *}
+        https://phitter.io/distributions/continuous/inverse_gaussian
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/inverse_gaussian_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/semicircular.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 import numpy
-import scipy.stats
+import scipy.special
 
 
-class INVERSE_GAUSSIAN_3P:
+class SEMICIRCULAR:
     """
-    Inverse Gaussian distribution
-    Also known like Wald distribution
-    Parameters INVERSE_GAUSSIAN_3P distribution: {"mu": *, "lambda": *, "loc": *}
-    https://phitter.io/distributions/continuous/inverse_gaussian_3p
+    Semicicrcular Distribution
+    https://phitter.io/distributions/continuous/semicircular
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the INVERSE_GAUSSIAN_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters INVERSE_GAUSSIAN_3P distribution: {"mu": *, "lambda": *, "loc": *}
+        Initializes the SEMICIRCULAR distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters SEMICIRCULAR distribution: {"loc": *, "R": *}
+        https://phitter.io/distributions/continuous/semicircular
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
-        self.mu = self.parameters["mu"]
-        self.lambda_ = self.parameters["lambda"]
         self.loc = self.parameters["loc"]
+        self.R = self.parameters["R"]
 
     @property
     def name(self):
-        return "inverse_gaussian_3p"
+        return "semicircular"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"mu": 9, "lambda": 77, "loc": 60}
+        return {"loc": 19, "R": 5}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        # result = scipy.stats.norm.cdf(numpy.sqrt(self.lambda_ / (x - self.loc)) * (((x - self.loc) / self.mu) - 1)) + numpy.exp(2 * self.lambda_ / self.mu) * scipy.stats.norm.cdf(-numpy.sqrt(self.lambda_ / (x - self.loc)) * (((x - self.loc) / self.mu) + 1))
-        result = scipy.stats.invgauss.cdf(x, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
+        z = lambda t: t - self.loc
+        result = 0.5 + z(x) * numpy.sqrt(self.R**2 - z(x) ** 2) / (numpy.pi * self.R**2) + numpy.arcsin(z(x) / self.R) / numpy.pi
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        # result = numpy.sqrt(self.lambda_ / (2 * numpy.pi * (x - self.loc) ** 3)) * numpy.exp(-(self.lambda_ * ((x - self.loc) - self.mu) ** 2) / (2 * self.mu**2 * (x - self.loc)))
-        result = scipy.stats.invgauss.pdf(x, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
+        z = lambda t: t - self.loc
+        result = 2 * numpy.sqrt(self.R**2 - z(x) ** 2) / (numpy.pi * self.R**2)
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = scipy.stats.invgauss.ppf(u, self.mu / self.lambda_, loc=self.loc, scale=self.lambda_)
+        result = self.loc + self.R * (2 * scipy.special.betaincinv(1.5, 1.5, u) - 1)
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -80,92 +78,96 @@
         return None
 
     @property
     def mean(self) -> float:
         """
         Parametric mean
         """
-        return self.mu + self.loc
+        return self.loc
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return self.mu**3 / self.lambda_
+        return (self.R * self.R) / 4
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
 
     @property
     def skewness(self) -> float:
         """
         Parametric skewness
         """
-        return 3 * numpy.sqrt(self.mu / self.lambda_)
+        return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 15 * (self.mu / self.lambda_) + 3
+        return 2
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
 
     @property
     def mode(self) -> float:
         """
         Parametric mode
         """
-        return self.loc + self.mu * (numpy.sqrt(1 + (9 * self.mu * self.mu) / (4 * self.lambda_ * self.lambda_)) - (3 * self.mu) / (2 * self.lambda_))
+        return self.loc
 
     @property
     def num_parameters(self) -> int:
         """
         Number of parameters of the distribution
         """
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
-        v1 = self.mu > 0
-        v2 = self.lambda_ > 0
-        return v1 and v2
+        v1 = self.R > 0
+        return v1
 
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures : dict
             {"mu": * , "variance": * , "skewness": * , "kurtosis": * , "data": * }
 
         Returns
         =======
-        parameters: {"mu": *, "lambda": *, "loc": *}
+        parameters: {"loc": *, "R": *}
         """
-        mu = 3 * numpy.sqrt(continuous_measures.variance / (continuous_measures.skewness**2))
-        lambda_ = mu**3 / continuous_measures.variance
-        loc = continuous_measures.mean - mu
+        loc = continuous_measures.mean
+        R = numpy.sqrt(4 * continuous_measures.variance)
+
+        ## Correction from domain  - R < x < R
+        d1 = (loc - R) - continuous_measures.min
+        d2 = continuous_measures.max - (loc + R)
+        delta = max(max(d1, 0), max(d2, 0)) + 1e-2
+        R = R + delta
+        parameters = {"loc": loc, "R": R}
 
-        parameters = {"mu": mu, "lambda": lambda_, "loc": loc}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
@@ -175,18 +177,18 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_inverse_gaussian_3p.txt"
+    path = "../continuous_distributions_sample/sample_semicircular.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = INVERSE_GAUSSIAN_3P(continuous_measures)
+    distribution = SEMICIRCULAR(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/johnson_sb.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/johnson_sb.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/johnson_sb
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the JOHNSON_SB distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters JOHNSON_SB distribution: {"xi": *, "lambda": *, "gamma": *, "delta": *}
+        https://phitter.io/distributions/continuous/johnson_sb
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -172,15 +173,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated with the method proposed in [1].
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"xi": *, "lambda": *, "gamma": *, "delta": *}
             {"xi": * , "lambda": * , "gamma": * , "delta": * }
 
         References
@@ -204,15 +205,15 @@
         xi_ = 0.5 * (x3 + x2) - 0.5 * lambda_ + p * (p / n - p / m) / (2 * (p**2 / (m * n) - 1))
         delta_ = z / numpy.arccosh(0.5 * numpy.sqrt((1 + p / m) * (1 + p / n)))
         gamma_ = delta_ * numpy.arcsinh((p / n - p / m) * numpy.sqrt((1 + p / m) * (1 + p / n) - 4) / (2 * (p**2 / (m * n) - 1)))
 
         parameters = {"xi": xi_, "lambda": lambda_, "gamma": gamma_, "delta": delta_}
 
         ## Scipy parameters
-        scipy_params = scipy.stats.johnsonsb.fit(continuous_measures.data)
+        scipy_params = scipy.stats.johnsonsb.fit(continuous_measures.data_to_fit)
         parameters = {"xi": scipy_params[2], "lambda": scipy_params[3], "gamma": scipy_params[0], "delta": scipy_params[1]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/johnson_su.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/johnson_su.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/johnson_su
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the JOHNSON_SU distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters JOHNSON_SU distribution: {"xi": *, "lambda": *, "gamma": *, "delta": *}
+        https://phitter.io/distributions/continuous/johnson_su
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/kumaraswamy.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/kumaraswamy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/kumaraswamy
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the KUMARASWAMY distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters KUMARASWAMY distribution: {"alpha": *, "beta": *, "min": *, "max": *}
+        https://phitter.io/distributions/continuous/kumaraswamy
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -175,15 +176,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *, "min": *, "max": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -207,18 +208,18 @@
             eq3 = parametric_skewness - continuous_measures.skewness
             eq4 = parametric_kurtosis - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3, eq4)
 
         # solution = scipy.optimize.fsolve(equations, (1, 1, 1, 1), continuous_measures)
         l = continuous_measures.min - 3 * abs(continuous_measures.min)
-        bnds = ((0, 0, l, l), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, 0, l, l), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
         x0 = (1, 1, 1, 1)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
 
         parameters = {"alpha": solution.x[0], "beta": solution.x[1], "min": solution.x[2], "max": solution.x[3]}
         return parameters
 
 
 if __name__ == "__main__":
     ## Import function to get continuous_measures
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/laplace.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/laplace.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     https://phitter.io/distributions/continuous/laplace
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LAPLACE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LAPLACE distribution: {"mu": *, "b": *}
+        https://phitter.io/distributions/continuous/laplace
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -139,15 +140,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"mu": *, "b": *}
         """
         mu = continuous_measures.mean
         b = numpy.sqrt(continuous_measures.variance / 2)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/levy.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/levy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/levy
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LEVY distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LEVY distribution: {"mu": *, "c": *}
+        https://phitter.io/distributions/continuous/levy
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -149,15 +150,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"mu": *, "c": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     ## Variables declaration
@@ -169,22 +170,22 @@
 
         #     ## System Equations
         #     eq1 = parametric_median - continuous_measures.median
         #     eq2 = parametric_mode - continuous_measures.mode
 
         #     return (eq1, eq2)
 
-        # bnds = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
+        # bounds = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
         # x0 = (1, 1)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # print(solution.x)
         # parameters = {"mu": solution.x[0], "c": solution.x[1]}
 
-        scipy_params = scipy.stats.levy.fit(continuous_measures.data)
+        scipy_params = scipy.stats.levy.fit(continuous_measures.data_to_fit)
 
         ## Results
         parameters = {"mu": scipy_params[0], "c": scipy_params[1]}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/loggamma.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/loggamma.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/loggamma
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LOGGAMMA distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LOGGAMMA distribution: {"c": *, "mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/loggamma
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -153,15 +154,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"c": *, "mu": *, "sigma": *}
         """
 
         def equations(initial_solution, data_mean, data_variance, data_skewness):
@@ -177,18 +178,18 @@
             eq1 = parametric_mean - data_mean
             eq2 = parametric_variance - data_variance
             eq3 = parametric_skewness - data_skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3)
 
-        bnds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
         x0 = (1, 1, 1)
         args = (continuous_measures.mean, continuous_measures.variance, continuous_measures.skewness)
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"c": solution.x[0], "mu": solution.x[1], "sigma": solution.x[2]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
@@ -239,18 +240,18 @@
         eq2 = parametric_variance - data_variance
         eq3 = parametric_skewness - data_skewness
         # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
         return (eq1, eq2, eq3)
 
     ti = time.time()
-    bnds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
+    bounds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
     x0 = (1, 1, 1)
     args = (continuous_measures.mean, continuous_measures.variance, continuous_measures.skewness)
-    solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+    solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
     parameters = {"c": solution.x[0], "mu": solution.x[1], "sigma": solution.x[2]}
     print(parameters)
     print("Solve equations time: ", time.time() - ti)
 
     ti = time.time()
     scipy_params = scipy.stats.loggamma.fit(data)
     parameters = {"c": scipy_params[0], "mu": scipy_params[1], "sigma": scipy_params[2]}
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/logistic.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/normal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import numpy
 import scipy.special
 import scipy.stats
 
 
-class LOGISTIC:
+class NORMAL:
     """
-    Logistic distribution
-    Parameters LOGISTIC distribution: {"mu": *, "sigma": *}
-    https://phitter.io/distributions/continuous/logistic
+    Normal distribution
+    Parameters NORMAL distribution: {"mu": *, "sigma": *}
+    https://phitter.io/distributions/continuous/normal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the LOGISTIC distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters LOGISTIC distribution: {"mu": *, "sigma": *}
+        Initializes the NORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters NORMAL distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/normal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -25,41 +26,41 @@
             self.parameters = self.parameters_example
 
         self.mu = self.parameters["mu"]
         self.sigma = self.parameters["sigma"]
 
     @property
     def name(self):
-        return "logistic"
+        return "normal"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"mu": 9, "sigma": 5}
+        return {"mu": 5, "sigma": 3}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        z = lambda t: numpy.exp(-(t - self.mu) / self.sigma)
-        result = 1 / (1 + z(x))
+        # result = scipy.stats.norm.cdf((x - self.mu) / self.sigma)
+        z = lambda t: (t - self.mu) / self.sigma
+        result = 0.5 * (1 + scipy.special.erf(z(x) / numpy.sqrt(2)))
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        z = lambda t: numpy.exp(-(t - self.mu) / self.sigma)
-        result = z(x) / (self.sigma * (1 + z(x)) ** 2)
+        result = (1 / (self.sigma * numpy.sqrt(2 * numpy.pi))) * numpy.exp(-(((x - self.mu) ** 2) / (2 * self.sigma**2)))
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = self.mu + self.sigma * numpy.log(u / (1 - u))
+        result = self.mu + self.sigma * scipy.stats.norm.ppf(u)
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -86,15 +87,15 @@
         return self.mu
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return (self.sigma * self.sigma * numpy.pi * numpy.pi) / 3
+        return self.sigma * 3
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
@@ -107,15 +108,15 @@
         return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 4.2
+        return 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
@@ -144,27 +145,26 @@
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
-        continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+        continuous_measures : dict
+            {"mu": * , "variance": * , "skewness": * , "kurtosis": * , "data": * }
 
         Returns
         =======
         parameters: {"mu": *, "sigma": *}
         """
+
         mu = continuous_measures.mean
-        sigma = numpy.sqrt(3 * continuous_measures.variance / (numpy.pi**2))
+        sigma = continuous_measures.standard_deviation
 
-        ## Results
         parameters = {"mu": mu, "sigma": sigma}
-
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
@@ -174,18 +174,18 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_logistic.txt"
+    path = "../continuous_distributions_sample/sample_normal.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = LOGISTIC(continuous_measures)
+    distribution = NORMAL(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/loglogistic.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/loglogistic.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/loglogistic
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LOGLOGISTIC distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LOGLOGISTIC distribution: {"alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/loglogistic
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -163,15 +164,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *}
         """
         # def equations(initial_solution, data_mean, data_variance, data_skewness):
         #     alpha, beta = initial_solution
@@ -185,21 +186,21 @@
 
         #     ## System Equations
         #     eq1 = parametric_mean - data_mean
         #     eq2 = parametric_variance - data_variance
 
         #     return (eq1, eq2)
 
-        # bnds = ((0, 0), (numpy.inf, numpy.inf))
+        # bounds = ((0, 0), (numpy.inf, numpy.inf))
         # x0 = (continuous_measures.mean, 1 / continuous_measures.variance ** 0.5)
         # args = (continuous_measures.mean, continuous_measures.variance, continuous_measures.skewness)
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"alpha": solution.x[0], "beta": solution.x[1]}
 
-        scipy_params = scipy.stats.fisk.fit(continuous_measures.data)
+        scipy_params = scipy.stats.fisk.fit(continuous_measures.data_to_fit)
         parameters = {"alpha": scipy_params[2], "beta": scipy_params[0]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
@@ -251,18 +252,18 @@
         ## System Equations
         eq1 = parametric_mean - data_mean
         eq2 = parametric_variance - data_variance
 
         return (eq1, eq2)
 
     ti = time.time()
-    bnds = ((0, 0), (numpy.inf, numpy.inf))
+    bounds = ((0, 0), (numpy.inf, numpy.inf))
     x0 = (continuous_measures.mean, continuous_measures.variance)
     args = (continuous_measures.mean, continuous_measures.variance, continuous_measures.skewness)
-    solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+    solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
     parameters = {"alpha": solution.x[0], "beta": solution.x[1]}
     print(parameters)
     print("Solve equations time: ", time.time() - ti)
 
     ti = time.time()
     scipy_params = scipy.stats.fisk.fit(data)
     parameters = {"alpha": scipy_params[2], "beta": scipy_params[0]}
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/loglogistic_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/loglogistic_3p.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/loglogistic_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LOGLOGISTIC_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LOGLOGISTIC_3P distribution: {"loc": *, "alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/loglogistic_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -164,21 +165,21 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"loc": *, "alpha": *, "beta": *}
         """
-        scipy_params = scipy.stats.fisk.fit(continuous_measures.data)
+        scipy_params = scipy.stats.fisk.fit(continuous_measures.data_to_fit)
         parameters = {"loc": scipy_params[1], "alpha": scipy_params[2], "beta": scipy_params[0]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
@@ -231,19 +232,19 @@
         ## System Equations
         eq1 = parametric_mean - continuous_measures.mean
         eq2 = parametric_variance - continuous_measures.variance
         eq3 = parametric_median - continuous_measures.median
 
         return (eq1, eq2, eq3)
 
-    bnds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+    bounds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
     x0 = (continuous_measures.mean, continuous_measures.variance, continuous_measures.mean)
     args = [continuous_measures]
     ti = time.time()
-    solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+    solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
     parameters = {"alpha": solution.x[0], "beta": solution.x[1], "loc": solution.x[2]}
     print(parameters)
     print("Solve equations time: ", time.time() - ti)
 
     ti = time.time()
     scipy_params = scipy.stats.fisk.fit(data)
     parameters = {"alpha": scipy_params[2], "beta": scipy_params[0], "loc": scipy_params[1]}
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/lognormal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/lognormal.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/lognormal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the LOGNORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters LOGNORMAL distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/lognormal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/maxwell.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/maxwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/maxwell
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the MAXWELL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters MAXWELL distribution: {"alpha": *, "loc": *}
+        https://phitter.io/distributions/continuous/maxwell
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -146,15 +147,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "loc": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     alpha, loc = initial_solution
@@ -169,18 +170,18 @@
         #     eq1 = parametric_mean - continuous_measures.mean
         #     eq2 = parametric_variance - continuous_measures.variance
         #     # eq3 = parametric_mode  - continuous_measures.mode
         #     eq3 = parametric_median - continuous_measures.median
 
         #     return (eq1, eq2, eq3)
 
-        # bnds = ((0,  - numpy.inf), (numpy.inf, numpy.inf))
+        # bounds = ((0,  - numpy.inf), (numpy.inf, numpy.inf))
         # x0 = (1, continuous_measures.mean)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"alpha": solution.x[0], "loc": solution.x[1]}
 
         alpha = numpy.sqrt(continuous_measures.variance * numpy.pi / (3 * numpy.pi - 8))
         loc = continuous_measures.mean - 2 * alpha * numpy.sqrt(2 / numpy.pi)
         parameters = {"alpha": alpha, "loc": loc}
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/moyal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/moyal.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/moyal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the MOYAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters MOYAL distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/moyal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -169,18 +170,18 @@
 
         #     ## System Equations
         #     eq1 = parametric_mean - continuous_measures.mean
         #     eq2 = parametric_variance - continuous_measures.variance
 
         #     return (eq1, eq2)
 
-        # bnds = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
+        # bounds = ((-numpy.inf, 0), (numpy.inf, numpy.inf))
         # x0 = (continuous_measures.mean, 1)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
 
         sigma = numpy.sqrt(2 * continuous_measures.variance / (numpy.pi * numpy.pi))
         mu = continuous_measures.mean - sigma * (numpy.log(2) + 0.577215664901532)
 
         parameters = {"mu": mu, "sigma": sigma}
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/nakagami.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/nakagami.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/nakagami
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the NAKAGAMI distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters NAKAGAMI distribution: {"m": *, "omega": *}
+        https://phitter.io/distributions/continuous/nakagami
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -151,15 +152,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"m": *, "omega": *}
         """
         d = numpy.array(continuous_measures.data)
         E_x2 = sum(d * d) / len(d)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_chi_square.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_chi_square.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/non_central_chi_square
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the NON_CENTRAL_CHI_SQUARE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters NON_CENTRAL_CHI_SQUARE distribution: {"lambda": *, "n": *}
+        https://phitter.io/distributions/continuous/non_central_chi_square
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -167,15 +168,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *, "n": *}
         """
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
         #     lambda_, n = initial_solution
@@ -190,18 +191,18 @@
         #     eq1 = parametric_mean - continuous_measures.mean
         #     eq2 = parametric_variance - continuous_measures.variance
         #     # eq3 = parametric_skewness - continuous_measures.skewness
         #     # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
         #     return (eq1, eq2)
 
-        # bnds = ((0, 0), (numpy.inf, numpy.inf))
+        # bounds = ((0, 0), (numpy.inf, numpy.inf))
         # x0 = (continuous_measures.mean, 1)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"lambda": solution.x[0], "n": round(solution.x[1])}
 
         lambda_ = continuous_measures.variance / 2 - continuous_measures.mean
         n = 2 * continuous_measures.mean - continuous_measures.variance / 2
         parameters = {"lambda": lambda_, "n": n}
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_f.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/non_central_f
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the NON_CENTRAL_F distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters NON_CENTRAL_F distribution: {"lambda": *, "n1": *, "n2": *}
+        https://phitter.io/distributions/continuous/non_central_f
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -222,15 +223,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *, "n1": *, "n2": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -252,18 +253,18 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3)
 
-        bnds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, 0, 0), (numpy.inf, numpy.inf, numpy.inf))
         x0 = (continuous_measures.mean, 1, 10)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"lambda": solution.x[0], "n1": solution.x[1], "n2": solution.x[2]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/non_central_t_student.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/non_central_t_student.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/non_central_t_student    Hand-book on Statistical Distributions (pag.116) ... Christian Walck
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the NON_CENTRAL_T_STUDENT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters NON_CENTRAL_T_STUDENT distribution: {"lambda": *, "n": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/non_central_t_student
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -213,15 +214,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *, "n": *, "loc": *, "scale": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -243,18 +244,18 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             eq4 = parametric_kurtosis - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3, eq4)
 
-        bnds = ((0, 0, 0, 0), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, 0, 0, 0), (numpy.inf, numpy.inf, numpy.inf, numpy.inf))
         x0 = (1, 5, continuous_measures.mean, 1)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"lambda": solution.x[0], "n": solution.x[1], "loc": solution.x[2], "scale": solution.x[3]}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/normal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/logistic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import numpy
 import scipy.special
 import scipy.stats
 
 
-class NORMAL:
+class LOGISTIC:
     """
-    Normal distribution
-    Parameters NORMAL distribution: {"mu": *, "sigma": *}
-    https://phitter.io/distributions/continuous/normal
+    Logistic distribution
+    Parameters LOGISTIC distribution: {"mu": *, "sigma": *}
+    https://phitter.io/distributions/continuous/logistic
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the NORMAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters NORMAL distribution: {"mu": *, "sigma": *}
+        Initializes the LOGISTIC distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters LOGISTIC distribution: {"mu": *, "sigma": *}
+        https://phitter.io/distributions/continuous/logistic
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -25,41 +26,41 @@
             self.parameters = self.parameters_example
 
         self.mu = self.parameters["mu"]
         self.sigma = self.parameters["sigma"]
 
     @property
     def name(self):
-        return "normal"
+        return "logistic"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"mu": 5, "sigma": 3}
+        return {"mu": 9, "sigma": 5}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        # result = scipy.stats.norm.cdf((x - self.mu) / self.sigma)
-        z = lambda t: (t - self.mu) / self.sigma
-        result = 0.5 * (1 + scipy.special.erf(z(x) / numpy.sqrt(2)))
+        z = lambda t: numpy.exp(-(t - self.mu) / self.sigma)
+        result = 1 / (1 + z(x))
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        result = (1 / (self.sigma * numpy.sqrt(2 * numpy.pi))) * numpy.exp(-(((x - self.mu) ** 2) / (2 * self.sigma**2)))
+        z = lambda t: numpy.exp(-(t - self.mu) / self.sigma)
+        result = z(x) / (self.sigma * (1 + z(x)) ** 2)
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = self.mu + self.sigma * scipy.stats.norm.ppf(u)
+        result = self.mu + self.sigma * numpy.log(u / (1 - u))
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -86,15 +87,15 @@
         return self.mu
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return self.sigma * 3
+        return (self.sigma * self.sigma * numpy.pi * numpy.pi) / 3
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
@@ -107,15 +108,15 @@
         return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 3
+        return 4.2
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
@@ -144,26 +145,27 @@
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
-        continuous_measures : dict
-            {"mu": * , "variance": * , "skewness": * , "kurtosis": * , "data": * }
+        continuous_measures: MEASUREMESTS
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"mu": *, "sigma": *}
         """
-
         mu = continuous_measures.mean
-        sigma = continuous_measures.standard_deviation
+        sigma = numpy.sqrt(3 * continuous_measures.variance / (numpy.pi**2))
 
+        ## Results
         parameters = {"mu": mu, "sigma": sigma}
+
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
@@ -173,18 +175,18 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_normal.txt"
+    path = "../continuous_distributions_sample/sample_logistic.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = NORMAL(continuous_measures)
+    distribution = LOGISTIC(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/pareto_first_kind.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/pareto_first_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/pareto_first_kind
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the PARETO_FIRST_KIND distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters PARETO_FIRST_KIND distribution: {"alpha": *, "xm": *, "loc": *}
+        https://phitter.io/distributions/continuous/pareto_first_kind
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -166,15 +167,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "xm": *, "loc": *}
         """
 
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -198,21 +199,21 @@
         #     # eq3 = parametric_skewness - continuous_measures.skewness
         #     # eq3 = parametric_kurtosis  - continuous_measures.kurtosis
         #     eq3 = parametric_mode - continuous_measures.mode
         #     # eq3 = parametric_median - continuous_measures.median
 
         #     return (eq1, eq2, eq3)
 
-        # bnds = ((1, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+        # bounds = ((1, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
         # x0 = (1, continuous_measures.mean, continuous_measures.mean)
         # args = [continuous_measures]
-        # solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         # parameters = {"alpha": solution.x[0], "xm": solution.x[1], "loc": solution.x[2]}
 
-        scipy_params = scipy.stats.pareto.fit(continuous_measures.data)
+        scipy_params = scipy.stats.pareto.fit(continuous_measures.data_to_fit)
         parameters = {"xm": scipy_params[2], "alpha": scipy_params[0], "loc": scipy_params[1]}
 
         # # Solve system
         # m = 112.5
         # me = continuous_measures.median
         # mo = 110
         # v = 10.41
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/pareto_second_kind.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/pareto_second_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/pareto_second_kind
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the PARETO_SECOND_KIND distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters PARETO_SECOND_KIND distribution: {"alpha": *, "xm": *, "loc": *}
+        https://phitter.io/distributions/continuous/pareto_second_kind
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -165,15 +166,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "xm": *, "loc": *}
         """
 
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -198,31 +199,31 @@
         #     # eq3 = parametric_skewness - continuous_measures.skewness
         #     # eq3 = parametric_kurtosis  - continuous_measures.kurtosis
         #     # eq2 = parametric_mode - continuous_measures.mode
         #     eq3 = parametric_median - continuous_measures.median
 
         #     return (eq1, eq2, eq3)
 
-        # bnds = ((1, 0,  - numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+        # bounds = ((1, 0,  - numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
         # x0 = (7, 6, continuous_measures.mode)
         # args = ([continuous_measures])
-        # solution = scipy.optimize.least_squares(equations, x0, bounds = bnds, args=args)
+        # solution = scipy.optimize.least_squares(equations, x0=x0, bounds = bnds, args=args)
         # parameters = {"alpha": solution.x[0], "xm": solution.x[1], "loc": solution.x[2]}
 
         m = continuous_measures.mean
         # me = continuous_measures.median
         # mo = continuous_measures.mode
         v = continuous_measures.variance
 
-        loc = scipy.stats.lomax.fit(continuous_measures.data)[1]
+        loc = scipy.stats.lomax.fit(continuous_measures.data_to_fit)[1]
         xm = -((m - loc) * ((m - loc) ** 2 + v)) / ((m - loc) ** 2 - v)
         alpha = -(2 * v) / ((m - loc) ** 2 - v)
         parameters = {"xm": xm, "alpha": alpha, "loc": loc}
 
-        # scipy_params = scipy.stats.lomax.fit(continuous_measures.data)
+        # scipy_params = scipy.stats.lomax.fit(continuous_measures.data_to_fit)
         # parameters = {"xm": scipy_params[2] , "alpha": scipy_params[0], "loc": scipy_params[1]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/pert.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/pert.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/pert
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the PERT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters PERT distribution: {"a": *, "b": *, "c": *}
+        https://phitter.io/distributions/continuous/pert
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -104,26 +105,24 @@
         return numpy.sqrt(self.variance)
 
     @property
     def skewness(self) -> float:
         """
         Parametric skewness
         """
-        α1 = (4 * self.b + self.c - 5 * self.a) / (self.c - self.a)
-        α2 = (5 * self.c - self.a - 4 * self.b) / (self.c - self.a)
-        return (2 * (α2 - α1) * numpy.sqrt(α1 + α2 + 1)) / ((α1 + α2 + 2) * numpy.sqrt(α1 * α2))
+        return (2 * (self.alpha2 - self.alpha1) * numpy.sqrt(self.alpha1 + self.alpha2 + 1)) / ((self.alpha1 + self.alpha2 + 2) * numpy.sqrt(self.alpha1 * self.alpha2))
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        α1 = (4 * self.b + self.c - 5 * self.a) / (self.c - self.a)
-        α2 = (5 * self.c - self.a - 4 * self.b) / (self.c - self.a)
-        return (6 * ((α2 - α1) ** 2 * (α1 + α2 + 1) - α1 * α2 * (α1 + α2 + 2))) / (α1 * α2 * (α1 + α2 + 2) * (α1 + α2 + 3)) + 3
+        return (6 * ((self.alpha2 - self.alpha1) ** 2 * (self.alpha1 + self.alpha2 + 1) - self.alpha1 * self.alpha2 * (self.alpha1 + self.alpha2 + 2))) / (
+            self.alpha1 * self.alpha2 * (self.alpha1 + self.alpha2 + 2) * (self.alpha1 + self.alpha2 + 3)
+        ) + 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
@@ -186,20 +185,20 @@
             # eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
             eq5 = parametric_median - continuous_measures.median
 
             return (eq1, eq2, eq5)
 
         ## Parameters of equations system
-        bnds = ((-numpy.inf, continuous_measures.mean, continuous_measures.min), (continuous_measures.mean, numpy.inf, continuous_measures.max))
+        bounds = ((-numpy.inf, continuous_measures.mean, continuous_measures.min), (continuous_measures.mean, numpy.inf, continuous_measures.max))
         x0 = (continuous_measures.min, continuous_measures.mean, continuous_measures.max)
         args = [continuous_measures]
 
         ## Solve Equation system
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"a": solution.x[0], "b": solution.x[1], "c": solution.x[2]}
 
         ## Correction of parameters
         parameters["a"] = min(continuous_measures.min - 1e-3, parameters["a"])
         parameters["c"] = max(continuous_measures.max + 1e-3, parameters["c"])
 
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/power_function.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/power_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/power_function
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the POWER_FUNCTION distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters POWER_FUNCTION distribution: {"alpha": *, "a": *, "b": *}
+        https://phitter.io/distributions/continuous/power_function
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -180,15 +181,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "a": *, "b": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -210,18 +211,18 @@
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
             # eq5 = parametric_median - continuous_measures.median
 
             return (eq1, eq2, eq3)
 
-        bnds = ((0, -numpy.inf, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, -numpy.inf, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
         x0 = (1, 1, continuous_measures.max)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"alpha": solution.x[0], "a": solution.x[1], "b": continuous_measures.max + 1e-3}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/rayleigh.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/rayleigh.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/rayleigh
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the RAYLEIGH distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters RAYLEIGH distribution: {"gamma": *, "sigma": *}
+        https://phitter.io/distributions/continuous/rayleigh
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -144,22 +145,22 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"gamma": *, "sigma": *}
         """
         ## Scipy Rayleigh estimation
-        # scipy_params = scipy.stats.rayleigh.fit(continuous_measures.data)
+        # scipy_params = scipy.stats.rayleigh.fit(continuous_measures.data_to_fit)
         # parameters = {"gamma": scipy_params[0], "sigma": scipy_params[1]}
 
         ## Location and sigma solve system
         sigma = numpy.sqrt(continuous_measures.variance * 2 / (4 - numpy.pi))
         gamma = continuous_measures.mean - sigma * numpy.sqrt(numpy.pi / 2)
 
         parameters = {"gamma": gamma, "sigma": sigma}
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/reciprocal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/reciprocal.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     https://phitter.io/distributions/continuous/reciprocal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the RECIPROCAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters RECIPROCAL distribution: {"a": *, "b": *}
+        https://phitter.io/distributions/continuous/reciprocal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -158,15 +159,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *}
         """
 
         a = continuous_measures.min - 1e-8
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/rice.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/rice.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     https://phitter.io/distributions/continuous/rice
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the RICE distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters RICE distribution: {"v": *, "sigma": *}
+        https://phitter.io/distributions/continuous/rice
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -217,15 +218,15 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"v": *, "sigma": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -243,18 +244,18 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             # eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
             return (eq1, eq2)
 
-        bnds = ((0, 0), (numpy.inf, numpy.inf))
+        bounds = ((0, 0), (numpy.inf, numpy.inf))
         x0 = (continuous_measures.mean, numpy.sqrt(continuous_measures.variance))
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"v": solution.x[0], "sigma": solution.x[1]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/semicircular.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/t_student.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 import numpy
 import scipy.special
+import scipy.stats
 
 
-class SEMICIRCULAR:
+class T_STUDENT:
     """
-    Semicicrcular Distribution
-    https://phitter.io/distributions/continuous/semicircular
+    T distribution
+    Parameters T_STUDENT distribution: {"df": *}
+    https://phitter.io/distributions/continuous/t_student    Hand - book on  STATISTICAL  DISTRIBUTIONS  for  experimentalists (pag.143) ...  Christian Walck
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the SEMICIRCULAR distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters SEMICIRCULAR distribution: {"loc": *, "R": *}
+        Initializes the T_STUDENT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters T_STUDENT distribution: {"df": *}
+        https://phitter.io/distributions/continuous/t_student
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
-        self.loc = self.parameters["loc"]
-        self.R = self.parameters["R"]
+        self.df = self.parameters["df"]
 
     @property
     def name(self):
-        return "semicircular"
+        return "t_student"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"loc": 19, "R": 5}
+        return {"df": 8}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        z = lambda t: t - self.loc
-        result = 0.5 + z(x) * numpy.sqrt(self.R**2 - z(x) ** 2) / (numpy.pi * self.R**2) + numpy.arcsin(z(x) / self.R) / numpy.pi
+        # result = scipy.stats.t.cdf(x, self.df)
+        result = scipy.special.betainc(self.df / 2, self.df / 2, (x + numpy.sqrt(x * x + self.df)) / (2 * numpy.sqrt(x * x + self.df)))
         return result
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        z = lambda t: t - self.loc
-        result = 2 * numpy.sqrt(self.R**2 - z(x) ** 2) / (numpy.pi * self.R**2)
+        # result = scipy.stats.t.pdf(x, self.df)
+        result = (1 / (numpy.sqrt(self.df) * scipy.special.beta(0.5, self.df / 2))) * (1 + x * x / self.df) ** (-(self.df + 1) / 2)
         return result
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = self.loc + self.R * (2 * scipy.special.betaincinv(1.5, 1.5, u) - 1)
+        # result = scipy.stats.t.ppf(u, self.df)
+        result = numpy.sign(u - 0.5) * numpy.sqrt(
+            self.df * (1 - scipy.special.betaincinv(self.df / 2, 0.5, 2 * numpy.min([u, 1 - u]))) / scipy.special.betaincinv(self.df / 2, 0.5, 2 * numpy.min([u, 1 - u]))
+        )
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -77,22 +82,22 @@
         return None
 
     @property
     def mean(self) -> float:
         """
         Parametric mean
         """
-        return self.loc
+        return 0
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return (self.R * self.R) / 4
+        return self.df / (self.df - 2)
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
@@ -105,68 +110,62 @@
         return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 2
+        return 6 / (self.df - 4) + 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
 
     @property
     def mode(self) -> float:
         """
         Parametric mode
         """
-        return self.loc
+        return 0
 
     @property
     def num_parameters(self) -> int:
         """
         Number of parameters of the distribution
         """
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
-        v1 = self.R > 0
+        v1 = self.df > 0
         return v1
 
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
-        The parameters are calculated by formula.
+        The parameters are calculated by solving the equations of the measures expected
+        for this distribution.The number of equations to consider is equal to the number
+        of parameters.
 
         Parameters
         ==========
-        continuous_measures : dict
-            {"mu": * , "variance": * , "skewness": * , "kurtosis": * , "data": * }
+        continuous_measures: MEASUREMESTS
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
-        parameters: {"loc": *, "R": *}
+        parameters: {"df": *}
         """
-        loc = continuous_measures.mean
-        R = numpy.sqrt(4 * continuous_measures.variance)
-
-        ## Correction from domain  - R < x < R
-        d1 = (loc - R) - continuous_measures.min
-        d2 = continuous_measures.max - (loc + R)
-        delta = max(max(d1, 0), max(d2, 0)) + 1e-2
-        R = R + delta
-        parameters = {"loc": loc, "R": R}
-
+        df = 2 * continuous_measures.variance / (continuous_measures.variance - 1)
+        parameters = {"df": df}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
@@ -176,18 +175,18 @@
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_semicircular.txt"
+    path = "../continuous_distributions_sample/sample_t_student.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = SEMICIRCULAR(continuous_measures)
+    distribution = T_STUDENT(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/t_student.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/uniform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,60 @@
 import numpy
-import scipy.special
-import scipy.stats
 
 
-class T_STUDENT:
+class UNIFORM:
     """
-    T distribution
-    Parameters T_STUDENT distribution: {"df": *}
-    https://phitter.io/distributions/continuous/t_student    Hand - book on  STATISTICAL  DISTRIBUTIONS  for  experimentalists (pag.143) ...  Christian Walck
+    Uniform distribution
+    Parameters UNIFORM distribution: {"a": *, "b": *}
+    https://phitter.io/distributions/continuous/uniform
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the T_STUDENT distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters T_STUDENT distribution: {"df": *}
+        Initializes the UNIFORM distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Parameters UNIFORM distribution: {"a": *, "b": *}
+        https://phitter.io/distributions/continuous/uniform
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
-        self.df = self.parameters["df"]
+        self.a = self.parameters["a"]
+        self.b = self.parameters["b"]
 
     @property
     def name(self):
-        return "t_student"
+        return "uniform"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"df": 8}
+        return {"a": 50, "b": 299}
 
     def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        # result = scipy.stats.t.cdf(x, self.df)
-        result = scipy.special.betainc(self.df / 2, self.df / 2, (x + numpy.sqrt(x * x + self.df)) / (2 * numpy.sqrt(x * x + self.df)))
-        return result
+        return (x - self.a) / (self.b - self.a)
 
     def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Probability density function
         """
-        # result = scipy.stats.t.pdf(x, self.df)
-        result = (1 / (numpy.sqrt(self.df) * scipy.special.beta(0.5, self.df / 2))) * (1 + x * x / self.df) ** (-(self.df + 1) / 2)
-        return result
+        return 1 / (self.b - self.a)
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        # result = scipy.stats.t.ppf(u, self.df)
-        result = numpy.sign(u - 0.5) * numpy.sqrt(
-            self.df * (1 - scipy.special.betaincinv(self.df / 2, 0.5, 2 * numpy.min([u, 1 - u]))) / scipy.special.betaincinv(self.df / 2, 0.5, 2 * numpy.min([u, 1 - u]))
-        )
+        result = self.a + u * (self.b - self.a)
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -81,22 +74,22 @@
         return None
 
     @property
     def mean(self) -> float:
         """
         Parametric mean
         """
-        return 0
+        return (self.a + self.b) / 2
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return self.df / (self.df - 2)
+        return (self.b - self.a) ** 2 / 12
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
@@ -109,62 +102,64 @@
         return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 6 / (self.df - 4) + 3
+        return 3 - 6 / 5
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
 
     @property
     def mode(self) -> float:
         """
         Parametric mode
         """
-        return 0
+        return None
 
     @property
     def num_parameters(self) -> int:
         """
         Number of parameters of the distribution
         """
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
-        v1 = self.df > 0
+        v1 = self.b > self.a
         return v1
 
     def get_parameters(self, continuous_measures) -> dict[str, float | int]:
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
-        The parameters are calculated by solving the equations of the measures expected
-        for this distribution.The number of equations to consider is equal to the number
-        of parameters.
+        The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
-        parameters: {"df": *}
+        parameters: {"a": *, "b": *}
         """
-        df = 2 * continuous_measures.variance / (continuous_measures.variance - 1)
-        parameters = {"df": df}
+
+        a = continuous_measures.min - 1e-8
+        b = continuous_measures.max + 1e-8
+
+        parameters = {"a": a, "b": b}
+
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
@@ -173,19 +168,20 @@
     ## Import function to get continuous_measures
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
+    path = "../continuous_distributions_sample/sample_uniform.txt"
+
     ## Distribution class
-    path = "../continuous_distributions_sample/sample_t_student.txt"
     data = get_data(path)
     continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = T_STUDENT(continuous_measures)
+    distribution = UNIFORM(continuous_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
     print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/t_student_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/t_student_3p.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/t_student_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the T_STUDENT_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters T_STUDENT_3P distribution: {"df": *, "loc": *, "scale": *}
+        https://phitter.io/distributions/continuous/t_student_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -151,22 +152,22 @@
         The parameters are calculated by solving the equations of the measures expected
         for this distribution.The number of equations to consider is equal to the number
         of parameters.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"df": *, "loc": *, "scale": *}
         """
         ## Scipy parameters
-        scipy_params = scipy.stats.t.fit(continuous_measures.data)
+        scipy_params = scipy.stats.t.fit(continuous_measures.data_to_fit)
         parameters = {"df": scipy_params[0], "loc": scipy_params[1], "scale": scipy_params[2]}
 
         # loc = continuous_measures.mean
         # df = 4 + 6 / (continuous_measures.kurtosis - 3)
         # scale = numpy.sqrt(continuous_measures.variance * (df + 2) / df)
         # parameters = {"df": df, "loc": loc, "scale": scale}
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/trapezoidal.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/trapezoidal.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/trapezoidal
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the TRAPEZOIDAL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters TRAPEZOIDAL distribution: {"a": *, "b": *, "c": *, "d": *}
+        https://phitter.io/distributions/continuous/trapezoidal
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -190,15 +191,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *, "c": *, "d": *}
         """
 
         def equations(initial_solution, continuous_measures, a, d):
@@ -217,16 +218,16 @@
 
             return (eq1, eq2)
 
         a = continuous_measures.min - 1e-3
         d = continuous_measures.max + 1e-3
 
         x0 = [(d + a) * 0.25, (d + a) * 0.75]
-        bnds = ((a, a), (d, d))
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=([continuous_measures, a, d]))
+        bounds = ((a, a), (d, d))
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=([continuous_measures, a, d]))
 
         parameters = {"a": a, "b": solution.x[0], "c": solution.x[1], "d": d}
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/triangular.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/triangular.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     https://phitter.io/distributions/continuous/triangular
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the TRIANGULAR distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters TRIANGULAR distribution: {"a": *, "b": *, "c": *}
+        https://phitter.io/distributions/continuous/triangular
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -164,15 +165,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *, "c": *}
         """
         ## Solve equations for estimation parameters
         # def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -206,15 +207,15 @@
         # v = (q_15_16 - q_3_4) ** 2
 
         # a = 2 * q_1_16 - q_1_4
         # b = 2 * q_15_16 - q_3_4
         # c = (u * b + v * a) / (u + v)
 
         # Scipy parameters of distribution
-        # scipy_params = scipy.stats.triang.fit(continuous_measures.data)
+        # scipy_params = scipy.stats.triang.fit(continuous_measures.data_to_fit)
         # a = scipy_params[1]
         # b = scipy_params[1] + scipy_params[2]
         # c = scipy_params[1] + scipy_params[2] * scipy_params[0]
 
         parameters = {"a": a, "b": b, "c": c}
         return parameters
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/uniform.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/uniform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 import numpy
 
 
 class UNIFORM:
     """
     Uniform distribution
     Parameters UNIFORM distribution: {"a": *, "b": *}
-    https://phitter.io/distributions/continuous/uniform
+    https://phitter.io/distributions/discrete/uniform
     """
 
-    def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+    def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the UNIFORM distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
-        Parameters UNIFORM distribution: {"a": *, "b": *}
-        """
-        if continuous_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
-        if continuous_measures != None:
-            self.parameters = self.get_parameters(continuous_measures)
+        Initializes the UNIFORM distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The UNIFORM distribution parameters are: {"a": *, "b": *}.
+        https://phitter.io/distributions/continuous/uniform
+        """
+        if discrete_measures is None and parameters is None and init_parameters_examples == False:
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
+        if discrete_measures != None:
+            self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
         self.a = self.parameters["a"]
         self.b = self.parameters["b"]
 
     @property
     def name(self):
         return "uniform"
 
     @property
     def parameters_example(self) -> dict[str, int | float]:
-        return {"a": 50, "b": 299}
+        return {"a": 3, "b": 10}
 
-    def cdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
+    def cdf(self, x: int | numpy.ndarray) -> float | numpy.ndarray:
         """
         Cumulative distribution function
         """
-        return (x - self.a) / (self.b - self.a)
+        return (x - self.a + 1) / (self.b - self.a + 1)
 
-    def pdf(self, x: float | numpy.ndarray) -> float | numpy.ndarray:
+    def pmf(self, x: int | numpy.ndarray) -> float | numpy.ndarray:
         """
-        Probability density function
+        Probability mass function
         """
-        return 1 / (self.b - self.a)
+        if type(x) == int:
+            return 1 / (self.b - self.a + 1)
+        return numpy.full(len(x), 1 / (self.b - self.a + 1))
 
     def ppf(self, u: float | numpy.ndarray) -> float | numpy.ndarray:
         """
         Percent point function. Inverse of Cumulative distribution function. If CDF[x] = u => PPF[u] = x
         """
-        result = self.a + u * (self.b - self.a)
+        result = numpy.ceil(u * (self.b - self.a + 1) + self.a - 1)
         return result
 
     def sample(self, n: int, seed: int | None = None) -> numpy.ndarray:
         """
         Sample of n elements of ditribution
         """
         if seed:
@@ -80,15 +83,15 @@
         return (self.a + self.b) / 2
 
     @property
     def variance(self) -> float:
         """
         Parametric variance
         """
-        return (self.b - self.a) ** 2 / 12
+        return ((self.b - self.a + 1) * (self.b - self.a + 1) - 1) / 12
 
     @property
     def standard_deviation(self) -> float:
         """
         Parametric standard deviation
         """
         return numpy.sqrt(self.variance)
@@ -101,15 +104,15 @@
         return 0
 
     @property
     def kurtosis(self) -> float:
         """
         Parametric kurtosis
         """
-        return 3 - 6 / 5
+        return ((-6 / 5) * ((self.b - self.a + 1) * (self.b - self.a + 1) + 1)) / ((self.b - self.a + 1) * (self.b - self.a + 1) - 1) + 3
 
     @property
     def median(self) -> float:
         """
         Parametric median
         """
         return self.ppf(0.5)
@@ -129,65 +132,64 @@
         return len(self.parameters)
 
     def parameter_restrictions(self) -> bool:
         """
         Check parameters restrictions
         """
         v1 = self.b > self.a
-        return v1
+        v2 = type(self.b) == int
+        v3 = type(self.a) == int
+        return v1 and v2 and v3
 
-    def get_parameters(self, continuous_measures) -> dict[str, float | int]:
+    def get_parameters(self, discrete_measures) -> dict[str, float | int]:
         """
-        Calculate proper parameters of the distribution from sample continuous_measures.
+        Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
-        continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+        discrete_measures: MEASUREMESTS
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"a": *, "b": *}
         """
-
-        a = continuous_measures.min - 1e-8
-        b = continuous_measures.max + 1e-8
-
+        a = round(discrete_measures.min)
+        b = round(discrete_measures.max)
         parameters = {"a": a, "b": b}
-
         return parameters
 
 
 if __name__ == "__main__":
     import sys
 
     sys.path.append("../")
-    from continuous_measures import CONTINUOUS_MEASURES
+    from discrete_measures import DISCRETE_MEASURES
 
-    ## Import function to get continuous_measures
-    def get_data(path: str) -> list[float]:
+    ## Import function to get discrete_measures
+    def get_data(path: str) -> list[int]:
         sample_distribution_file = open(path, "r")
-        data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
+        data = [int(x) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
-    path = "../continuous_distributions_sample/sample_uniform.txt"
+    path = "../discrete_distributions_sample/sample_uniform.txt"
 
     ## Distribution class
     data = get_data(path)
-    continuous_measures = CONTINUOUS_MEASURES(data)
-    distribution = UNIFORM(continuous_measures)
+    discrete_measures = DISCRETE_MEASURES(data)
+    distribution = UNIFORM(discrete_measures)
 
     print(f"{distribution.name} distribution")
     print(f"Parameters: {distribution.parameters}")
-    print(f"CDF: {distribution.cdf(continuous_measures.mean)} {distribution.cdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
-    print(f"PDF: {distribution.pdf(continuous_measures.mean)} {distribution.pdf(numpy.array([continuous_measures.mean, continuous_measures.mean]))}")
+    print(f"CDF: {distribution.cdf(int(discrete_measures.mean))} {distribution.cdf(numpy.array([int(discrete_measures.mean), int(discrete_measures.mean)]))}")
+    print(f"PMF: {distribution.pmf(int(discrete_measures.mean))} {distribution.pmf(numpy.array([int(discrete_measures.mean), int(discrete_measures.mean)]))}")
     print(f"PPF: {distribution.ppf(0.5)} {distribution.ppf(numpy.array([0.5, 0.5]))} - V: {distribution.cdf(distribution.ppf(0.5))}")
     print(f"SAMPLE: {distribution.sample(5)}")
     print(f"\nSTATS")
-    print(f"mean: {distribution.mean} - {continuous_measures.mean}")
-    print(f"variance: {distribution.variance} - {continuous_measures.variance}")
-    print(f"skewness: {distribution.skewness} - {continuous_measures.skewness}")
-    print(f"kurtosis: {distribution.kurtosis} - {continuous_measures.kurtosis}")
-    print(f"median: {distribution.median} - {continuous_measures.median}")
-    print(f"mode: {distribution.mode} - {continuous_measures.mode}")
+    print(f"mean: {distribution.mean} - {discrete_measures.mean}")
+    print(f"variance: {distribution.variance} - {discrete_measures.variance}")
+    print(f"skewness: {distribution.skewness} - {discrete_measures.skewness}")
+    print(f"kurtosis: {distribution.kurtosis} - {discrete_measures.kurtosis}")
+    print(f"median: {distribution.median} - {discrete_measures.median}")
+    print(f"mode: {distribution.mode} - {discrete_measures.mode}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/weibull.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/weibull.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/weibull
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the WEIBULL distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters WEIBULL distribution: {"alpha": *, "beta": *}
+        https://phitter.io/distributions/continuous/weibull
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -164,15 +165,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "beta": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_distributions/weibull_3p.py` & `phitter-0.0.5/phitter/continuous/continuous_distributions/weibull_3p.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     https://phitter.io/distributions/continuous/weibull_3p
     """
 
     def __init__(self, continuous_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
         Initializes the WEIBULL_3P distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
         Parameters WEIBULL_3P distribution: {"alpha": *, "loc": *, "beta": *}
+        https://phitter.io/distributions/continuous/weibull_3p
         """
         if continuous_measures is None and parameters is None and init_parameters_examples == False:
             raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
         if continuous_measures != None:
             self.parameters = self.get_parameters(continuous_measures)
         if parameters != None:
             self.parameters = parameters
@@ -167,15 +168,15 @@
         """
         Calculate proper parameters of the distribution from sample continuous_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         continuous_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"alpha": *, "loc": *, "beta": *}
         """
 
         def equations(initial_solution: tuple[float], continuous_measures) -> tuple[float]:
@@ -195,18 +196,18 @@
             eq1 = parametric_mean - continuous_measures.mean
             eq2 = parametric_variance - continuous_measures.variance
             eq3 = parametric_skewness - continuous_measures.skewness
             # eq4 = parametric_kurtosis  - continuous_measures.kurtosis
 
             return (eq1, eq2, eq3)
 
-        bnds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((0, 0, -numpy.inf), (numpy.inf, numpy.inf, numpy.inf))
         x0 = (1, 1, continuous_measures.mean)
         args = [continuous_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"alpha": solution.x[0], "loc": solution.x[2], "beta": solution.x[1]}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_measures/continuous_measures.py` & `phitter-0.0.5/phitter/continuous/continuous_measures/continuous_measures.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,51 +5,53 @@
 
 class CONTINUOUS_MEASURES:
     def __init__(
         self,
         data: list[float | int],
         num_bins: int | None = None,
         confidence_level: float = 0.95,
+        subsample_estimation_size: int | None = None,
     ):
         self.data = numpy.sort(data)
         self.data_unique = numpy.unique(self.data)
-        self.length = len(self.data)
+        self.size = self.data.size
+        self.data_to_fit = self.data if subsample_estimation_size == None else numpy.random.choice(self.data, size=min(self.size, subsample_estimation_size), replace=False)
         self.min = self.data[0]
         self.max = self.data[-1]
         self.mean = numpy.mean(self.data)
         self.variance = numpy.var(self.data, ddof=1)
         self.standard_deviation = numpy.sqrt(self.variance)
         self.skewness = scipy.stats.moment(self.data, 3) / pow(self.standard_deviation, 3)
         self.kurtosis = scipy.stats.moment(self.data, 4) / pow(self.standard_deviation, 4)
         self.median = numpy.median(self.data)
         self.mode = self.calculate_mode()
         self.num_bins = num_bins if num_bins != None else len(numpy.histogram_bin_edges(self.data, bins="doane"))
         self.absolutes_frequencies, self.bin_edges = numpy.histogram(self.data, self.num_bins)
         self.densities_frequencies, _ = numpy.histogram(self.data, self.num_bins, density=True)
         self.central_values = (self.bin_edges[:-1] + self.bin_edges[1:]) / 2
-        self.idx_ks = numpy.concatenate([numpy.where(self.data[:-1] != self.data[1:])[0], [self.length - 1]])
-        self.Sn_ks = (numpy.arange(self.length) + 1) / self.length
+        self.idx_ks = numpy.concatenate([numpy.where(self.data[:-1] != self.data[1:])[0], [self.size - 1]])
+        self.Sn_ks = (numpy.arange(self.size) + 1) / self.size
         self.confidence_level = confidence_level
-        self.critical_value_ks = scipy.stats.kstwo.ppf(self.confidence_level, self.length)
-        self.critical_value_ad = self.ad_critical_value(self.confidence_level, self.length)
-        self.ecdf_frequencies = numpy.arange(1, len(self.data_unique) + 1) / len(self.data_unique)
-        self.qq_arr = (numpy.arange(1, self.length + 1) - 0.5) / self.length
+        self.critical_value_ks = scipy.stats.kstwo.ppf(self.confidence_level, self.size)
+        self.critical_value_ad = self.ad_critical_value(self.confidence_level, self.size)
+        self.ecdf_frequencies = numpy.searchsorted(self.data, self.data_unique, side="right") / self.data.size
+        self.qq_arr = (numpy.arange(1, self.size + 1) - 0.5) / self.size
 
     def __str__(self) -> str:
-        return str({"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
+        return str({"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
 
     def __repr__(self) -> str:
-        return str({"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
+        return str({"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
 
     def get_dict(self) -> str:
-        return {"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode}
+        return {"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode}
 
     def calculate_mode(self) -> float:
         distribution = scipy.stats.gaussian_kde(self.data)
-        # solution = scipy.optimize.shgo(lambda x: -distribution.pdf(x)[0], bounds=[(self.min, self.max)], n=100 * self.length)
+        # solution = scipy.optimize.shgo(lambda x: -distribution.pdf(x)[0], bounds=[(self.min, self.max)], n=100 * self.size)
         solution = scipy.optimize.minimize(lambda x: -distribution.pdf(x)[0], x0=[self.mean], bounds=[(self.min, self.max)])
         return solution.x[0]
 
     def critical_value_chi2(self, freedom_degrees: int):
         return scipy.stats.chi2.ppf(self.confidence_level, freedom_degrees)
 
     def adinf(self, z: float):
@@ -97,15 +99,15 @@
 
     ## Distribution class
     path = "../continuous_distributions_sample/sample_exponential.txt"
     data = get_data(path)
 
     continuous_measures = CONTINUOUS_MEASURES(data)
 
-    print(f"Length: {continuous_measures.length}")
+    print(f"Size: {continuous_measures.size}")
     print(f"Min: {continuous_measures.min}")
     print(f"Max: {continuous_measures.max}")
     print(f"Mean: {continuous_measures.mean}")
     print(f"Variance: {continuous_measures.variance}")
     print(f"Standard Deviation: {continuous_measures.standard_deviation}")
     print(f"Skewness: {continuous_measures.skewness}")
     print(f"Kurtosis: {continuous_measures.kurtosis}")
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_anderson_darling.py` & `phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_anderson_darling.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
            Journal of the American Statistical Association, 83(404), 1190 - 1191.
     .. [3] Lewis, P. A. (1961).
            Distribution of the Anderson - Darling statistic.
            The Annals of Mathematical Statistics, 1118 - 1124.
     """
 
     ## Parameters and preparations
-    N = continuous_measures.length
+    N = continuous_measures.size
 
     ## Calculation S
     S = numpy.sum(((2 * (numpy.arange(N) + 1) - 1) / N) * (numpy.log(distribution.cdf(continuous_measures.data)) + numpy.log(1 - distribution.cdf(continuous_measures.data[::-1]))))
 
     ## Calculation of indicators
     A2 = -N - S
     critical_value = continuous_measures.critical_value_ad
@@ -74,15 +74,15 @@
 
     def get_data(path: str) -> list[float]:
         sample_distribution_file = open(path, "r")
         data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
         sample_distribution_file.close()
         return data
 
-    for distribution_name, distribution_class in _ALL_CONTINUOUS_DISTRIBUTIONS.items():
+    for distribution_name, distribution_class in ALL_CONTINUOUS_DISTRIBUTIONS.items():
         print(distribution_name)
         path = f"../continuous_distributions_sample/sample_{distribution_name}.txt"
         data = get_data(path)
 
         ## Init a instance of class
         continuous_measures = CONTINUOUS_MEASURES(data)
         distribution = distribution_class(continuous_measures)
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_chi_square.py` & `phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_chi_square.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         4. rejected(bool):
             decision if the null hypothesis is rejected. If it is false, it can be
             considered that the sample is distributed according to the probability
             distribution. If it's true, no.
     """
 
     ## Parameters and preparations
-    N = continuous_measures.length
+    N = continuous_measures.size
     freedom_degrees = max(continuous_measures.num_bins - 1 - distribution.num_parameters, 1)
 
     ## Calculation of errors
     expected_values = N * (distribution.cdf(continuous_measures.bin_edges[1:]) - distribution.cdf(continuous_measures.bin_edges[:-1]))
     errors = ((continuous_measures.absolutes_frequencies - expected_values) ** 2) / expected_values
 
     ## Calculation of indicators
```

### Comparing `phitter-0.0.4/phitter/continuous/continuous_statistical_tests/continuous_test_kolmogorov_smirnov.py` & `phitter-0.0.5/phitter/continuous/continuous_statistical_tests/continuous_test_kolmogorov_smirnov.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         4. rejected(bool):
             decision if the null hypothesis is rejected. If it is false, it can be
             considered that the sample is distributed according to the probability
             distribution. If it's true, no.
     """
 
     ## Parameters and preparations
-    N = continuous_measures.length
+    N = continuous_measures.size
 
     ## Calculation of errors
     Fn = distribution.cdf(continuous_measures.data)
     errors = numpy.abs(continuous_measures.Sn_ks[continuous_measures.idx_ks] - Fn[continuous_measures.idx_ks])
 
     ## Calculation of indicators
     statistic_ks = numpy.max(errors)
```

### Comparing `phitter-0.0.4/phitter/continuous/phitter_continuous.py` & `phitter-0.0.5/phitter/continuous/phitter_continuous.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import concurrent.futures
+import random
+import re
 import sys
 import typing
 
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy
 import plotly.express as px
 import plotly.graph_objects as go
 import scipy.stats
 
 sys.path.append("../..")
 from phitter.continuous.continuous_distributions import ALL_CONTINUOUS_DISTRIBUTIONS
@@ -18,28 +22,45 @@
 class PHITTER_CONTINUOUS:
     def __init__(
         self,
         data: list[int | float] | numpy.ndarray,
         num_bins: int | None = None,
         confidence_level=0.95,
         minimum_sse=numpy.inf,
+        subsample_estimation_size: int | None = None,
         distributions_to_fit: list[str] | typing.Literal["all"] = "all",
+        exclude_distributions: list[str] | typing.Literal["any"] = "any",
     ):
-        if distributions_to_fit != "all":
+        if distributions_to_fit != "all" and exclude_distributions != "any":
+            raise Exception(f"Specify either distributions_to_fit or exclude_distributions, not both.")
+
+        if distributions_to_fit == "all" and exclude_distributions == "any":
+            self.distributions_to_fit = list(ALL_CONTINUOUS_DISTRIBUTIONS.keys())
+
+        if distributions_to_fit != "all" and exclude_distributions == "any":
             not_distributions_ids = [dist for dist in distributions_to_fit if dist not in ALL_CONTINUOUS_DISTRIBUTIONS.keys()]
             if len(not_distributions_ids) > 0:
                 raise Exception(f"{not_distributions_ids} not founded in continuous disributions")
+            self.distributions_to_fit = distributions_to_fit
+
+        if distributions_to_fit == "all" and exclude_distributions != "any":
+            not_distributions_ids = [dist for dist in exclude_distributions if dist not in ALL_CONTINUOUS_DISTRIBUTIONS.keys()]
+            if len(not_distributions_ids) > 0:
+                raise Exception(f"{not_distributions_ids} not founded in continuous disributions")
+            self.distributions_to_fit = [dist for dist in ALL_CONTINUOUS_DISTRIBUTIONS.keys() if dist not in exclude_distributions]
 
-        self.data = data
-        self.continuous_measures = CONTINUOUS_MEASURES(self.data, num_bins, confidence_level)
-        self.confidence_level = confidence_level
+        self.continuous_measures = CONTINUOUS_MEASURES(
+            data=data,
+            num_bins=num_bins,
+            confidence_level=confidence_level,
+            subsample_estimation_size=subsample_estimation_size,
+        )
         self.minimum_sse = minimum_sse
         self.distribution_results = {}
         self.none_results = {"test_statistic": None, "critical_value": None, "p_value": None, "rejected": None}
-        self.distributions_to_fit = list(ALL_CONTINUOUS_DISTRIBUTIONS.keys()) if distributions_to_fit == "all" else distributions_to_fit
         self.sorted_distributions_sse = None
         self.not_rejected_distributions = None
         self.distribution_instances = None
 
     def test(self, test_function, label: str, distribution):
         validation_test = False
         try:
@@ -103,24 +124,30 @@
             processing_results = list(executor.map(self.process_distribution, self.distributions_to_fit))
 
         processing_results = [r for r in processing_results if r is not None]
         self.sorted_distributions_sse = {distribution: results for distribution, results, _ in sorted(processing_results, key=lambda x: (-x[1]["n_test_passed"], x[1]["sse"]))}
         self.not_rejected_distributions = {distribution: results for distribution, results in self.sorted_distributions_sse.items() if results["n_test_passed"] > 0}
         self.distribution_instances = {distribution: instance for distribution, _, instance in processing_results}
 
-    def plot_histogram(
+    def parse_rgba_color(self, rgba_string):
+        rgba = re.match(r"rgba\((\d+),(\d+),(\d+),(\d*(?:\.\d+)?)\)", rgba_string)
+        r, g, b, a = map(float, rgba.groups())
+        return (r / 255, g / 255, b / 255, a)
+
+    def plot_histogram_plotly(
         self,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
+        plot_renderer: str | None,
     ):
         central_values = self.continuous_measures.central_values
         densities_frequencies = self.continuous_measures.densities_frequencies
 
         fig = go.Figure()
         fig.add_trace(go.Bar(x=central_values, y=densities_frequencies, marker_color=plot_bar_color, name="Data", showlegend=True))
         fig.update_layout(
@@ -130,28 +157,50 @@
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
             bargap=plot_bargap,
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_histogram_matplotlib(
+        self,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None = None,
+    ):
+        matplotlib.style.use("ggplot")
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.hist(self.continuous_measures.data, density=True, label="Data", bins=self.continuous_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
-    def plot_histogram_distributions_pdf(
+    def plot_histogram_distributions_pdf_plotly(
         self,
         n_distributions: int,
         n_distributions_visible: int,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
+        plot_renderer: str | None,
     ):
         central_values = self.continuous_measures.central_values
         densities_frequencies = self.continuous_measures.densities_frequencies
 
         fig = go.Figure()
         fig.add_trace(go.Bar(x=central_values, y=densities_frequencies, marker_color=plot_bar_color, showlegend=False, name="Data"))
 
@@ -167,40 +216,73 @@
                 fig.add_trace(go.Scatter(x=x_plot, y=y_plot, mode="lines", visible=is_visible, name=scatter_name, line=scatter_line))
             except Exception:
                 fig.add_trace(go.Scatter(x=x_plot, y=numpy.zeros(len(x_plot)), mode="lines", visible=is_visible, name=scatter_name, line=scatter_line))
 
         fig.update_layout(
             height=plot_height,
             width=plot_width,
-            title=f"{plot_title} - PDF DISTRIBUTIONS",
+            title=plot_title,
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
             bargap=plot_bargap,
         )
 
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_histogram_distributions_pdf_matplotlib(
+        self,
+        n_distributions: int,
+        n_distributions_visible: int,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.hist(self.continuous_measures.data, density=True, bins=self.continuous_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
+
+        x_plot = numpy.linspace(self.continuous_measures.min, self.continuous_measures.max, 1000)
+        for idx, (distribution_name, result) in enumerate(list(self.sorted_distributions_sse.items())[:n_distributions]):
+            y_plot = self.distribution_instances[distribution_name].pdf(x_plot)
+            distribution_sse = result["sse"]
+            is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+            scatter_name = f"{idx+1:02d}. {distribution_name}: {distribution_sse:.4E}{is_rejected}"
+            plt.plot(x_plot, y_plot, label=scatter_name, color=(random.uniform(0, 1), random.uniform(0, 1), random.uniform(0, 1)))
+
+        plt.title(f"{plot_title} - PDF DISTRIBUTIONS")
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
-    def plot_distribution_pdf(
+    def plot_distribution_pdf_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
         plot_line_color: str,
         plot_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         central_values = self.continuous_measures.central_values
         densities_frequencies = self.continuous_measures.densities_frequencies
 
@@ -229,35 +311,75 @@
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
             bargap=plot_bargap,
         )
 
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_distribution_pdf_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_line_color: str,
+        plot_line_width: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not founded")
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.hist(self.continuous_measures.data, density=True, label="Data", bins=self.continuous_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
 
-    def plot_ecdf(
+        x_plot = numpy.linspace(self.continuous_measures.min, self.continuous_measures.max, 1000)
+        y_plot = self.distribution_instances[distribution_name].pdf(x_plot)
+        distribution_sse = self.sorted_distributions_sse[distribution_name]["sse"]
+        is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+        scatter_name = f"{distribution_name}: {distribution_sse:.4E}{is_rejected}"
+        try:
+            plt.plot(x_plot, y_plot, label=scatter_name, color=self.parse_rgba_color(plot_line_color), linewidth=plot_line_width)
+        except Exception:
+            plt.plot(x_plot, numpy.zeros(len(x_plot)), label=scatter_name, color=self.parse_rgba_color(plot_line_color), linewidth=plot_line_width)
+
+        plt.title(f"{plot_title} - PDF {distribution_name.upper().replace('_', ' ')} DISTRIBUTION")
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def plot_ecdf_plotly(
         self,
         plot_title: str,
         plot_xaxis_title: str,
         plot_xaxis_min_offset: float,
         plot_xaxis_max_offset: float,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_line_color: str,
         plot_line_width: int,
         plot_line_name: str,
+        plot_renderer: str | None,
     ):
         fig = go.Figure()
         fig.add_trace(
             go.Scatter(
                 x=numpy.repeat(self.continuous_measures.data_unique, 2)[1:-1],
-                y=numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-1],
+                y=numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-2],
                 mode="lines",
                 name=plot_line_name,
                 line=dict(color=plot_line_color, width=plot_line_width),
                 showlegend=True,
             )
         )
         fig.update_layout(
@@ -269,17 +391,48 @@
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
             xaxis_range=[self.continuous_measures.min - plot_xaxis_min_offset, self.continuous_measures.max + plot_xaxis_max_offset],
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_ecdf_matplotlib(
+        self,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_xaxis_min_offset: float,
+        plot_xaxis_max_offset: float,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_line_color: str,
+        plot_line_width: int,
+        plot_line_name: str,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.plot(
+            numpy.repeat(self.continuous_measures.data_unique, 2)[1:-1],
+            numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-2],
+            label=plot_line_name,
+            color=self.parse_rgba_color(plot_line_color),
+            linewidth=plot_line_width,
+        )
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.xlim([self.continuous_measures.min - plot_xaxis_min_offset, self.continuous_measures.max + plot_xaxis_max_offset])
+        plt.show()
 
-    def plot_ecdf_distribution(
+    def plot_ecdf_distribution_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_xaxis_min_offset: float,
         plot_xaxis_max_offset: float,
         plot_yaxis_title: str,
@@ -287,20 +440,33 @@
         plot_height: int,
         plot_width: int,
         plot_empirical_line_color: str,
         plot_empirical_line_width: int,
         plot_empirical_line_name: str,
         plot_distribution_line_color: str,
         plot_distribution_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         fig = go.Figure()
 
+        # Línea empírica
+        fig.add_trace(
+            go.Scatter(
+                x=numpy.repeat(self.continuous_measures.data_unique, 2)[1:-1],
+                y=numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-1],
+                mode="lines",
+                name=plot_empirical_line_name,
+                line=dict(color=plot_empirical_line_color, width=plot_empirical_line_width),
+                showlegend=True,
+            )
+        )
+
         # Línea de la distribución
         x_plot = numpy.linspace(self.continuous_measures.min, self.continuous_measures.max, 1000)
         y_plot = self.distribution_instances[distribution_name].cdf(x_plot)
         distribution_sse = self.sorted_distributions_sse[distribution_name]["sse"]
         is_rejected = "✅" if distribution_name in self.not_rejected_distributions else ""
         try:
             fig.add_trace(
@@ -311,53 +477,90 @@
                     name=f"{distribution_name}: {distribution_sse:.4E}{is_rejected}",
                     line=dict(color=plot_distribution_line_color, width=plot_distribution_line_width),
                 )
             )
         except Exception:
             fig.add_trace(go.Scatter(x=x_plot, y=numpy.zeros(len(x_plot)), mode="lines", name=f"{distribution_name}: {distribution_sse:.4E}{is_rejected}"))
 
-        # Línea empírica
-        fig.add_trace(
-            go.Scatter(
-                x=numpy.repeat(self.continuous_measures.data_unique, 2)[1:-1],
-                y=numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-1],
-                mode="lines",
-                name=plot_empirical_line_name,
-                line=dict(color=plot_empirical_line_color, width=plot_empirical_line_width),
-                showlegend=True,
-            )
-        )
-
         fig.update_layout(
             height=plot_height,
             width=plot_width,
             title=f"{plot_title} - CDF {distribution_name.upper().replace('_', ' ')} DISTRIBUTION",
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
             xaxis_range=[self.continuous_measures.min - plot_xaxis_min_offset, self.continuous_measures.max + plot_xaxis_max_offset],
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_ecdf_distribution_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_xaxis_min_offset: float,
+        plot_xaxis_max_offset: float,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_empirical_line_color: str,
+        plot_empirical_line_width: int,
+        plot_empirical_line_name: str,
+        plot_distribution_line_color: str,
+        plot_distribution_line_width: int,
+        plot_renderer: str | None,
+    ):
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not founded")
+
+        matplotlib.style.use("ggplot")
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.plot(
+            numpy.repeat(self.continuous_measures.data_unique, 2)[1:-1],
+            numpy.repeat(self.continuous_measures.ecdf_frequencies, 2)[:-2],
+            label=plot_empirical_line_name,
+            color=self.parse_rgba_color(plot_empirical_line_color),
+            linewidth=plot_empirical_line_width,
+        )
+
+        x_plot = numpy.linspace(self.continuous_measures.min, self.continuous_measures.max, 1000)
+        y_plot = self.distribution_instances[distribution_name].cdf(x_plot)
+        distribution_sse = self.sorted_distributions_sse[distribution_name]["sse"]
+        is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+        scatter_name = f"{distribution_name}: {distribution_sse:.4E}{is_rejected}"
+        try:
+            plt.plot(x_plot, y_plot, label=scatter_name, color=self.parse_rgba_color(plot_distribution_line_color), linewidth=plot_distribution_line_width)
+        except Exception:
+            plt.plot(x_plot, numpy.zeros(len(x_plot)), label=scatter_name, color=self.parse_rgba_color(plot_distribution_line_color), linewidth=plot_distribution_line_width)
+
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.xlim([self.continuous_measures.min - plot_xaxis_min_offset, self.continuous_measures.max + plot_xaxis_max_offset])
+        plt.show()
 
-    def qq_plot(
+    def qq_plot_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         qq_marker_name: str,
         qq_marker_color: str,
         qq_marker_size: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         x = self.distribution_instances[distribution_name].ppf(self.continuous_measures.qq_arr)
         y = self.continuous_measures.data
 
@@ -371,31 +574,61 @@
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
 
-    def qq_plot_regression(
+    def qq_plot_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        qq_marker_name: str,
+        qq_marker_color: str,
+        qq_marker_size: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not found")
+
+        x = self.distribution_instances[distribution_name].ppf(self.continuous_measures.qq_arr)
+        y = self.continuous_measures.data
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.scatter(x, y, label=qq_marker_name, color=self.parse_rgba_color(qq_marker_color), s=qq_marker_size)
+        plt.title(f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION")
+        plt.xlabel(plot_xaxis_title)
+        plt.ylabel(plot_yaxis_title)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def qq_plot_regression_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         qq_marker_name: str,
         qq_marker_color: str,
         qq_marker_size: int,
         regression_line_name: str,
         regression_line_color: str,
         regression_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         x = self.distribution_instances[distribution_name].ppf(self.continuous_measures.qq_arr)
         y = self.continuous_measures.data
 
@@ -404,24 +637,62 @@
 
         fig = go.Figure()
         fig.add_trace(go.Scatter(x=x, y=y_reg, mode="lines", name=regression_line_name, line=dict(color=regression_line_color, width=regression_line_width)))
         fig.add_trace(go.Scatter(x=x, y=y, mode="markers", name=qq_marker_name, marker=dict(color=qq_marker_color, size=qq_marker_size)))
         fig.update_layout(
             height=plot_height,
             width=plot_width,
-            title=f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION <br><br><sup>Regression: {linear_regression.intercept:.4g} + x * {linear_regression.slope:.4g} • r = {linear_regression.rvalue:.4g}</sup>",
+            title=f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION <br><br><sup>Regression: {linear_regression.intercept:.4f} + x * {linear_regression.slope:.4f} • r = {linear_regression.rvalue:.4f}</sup>",
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=10),
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def qq_plot_regression_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        qq_marker_name: str,
+        qq_marker_color: str,
+        qq_marker_size: int,
+        regression_line_name: str,
+        regression_line_color: str,
+        regression_line_width: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not found")
+
+        x = self.distribution_instances[distribution_name].ppf(self.continuous_measures.qq_arr)
+        y = self.continuous_measures.data
+
+        linear_regression = scipy.stats.linregress(x, y)
+        y_reg = linear_regression.intercept + x * linear_regression.slope
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.plot(x, y_reg, label=regression_line_name, color=self.parse_rgba_color(regression_line_color), linewidth=regression_line_width)
+        plt.scatter(x, y, label=qq_marker_name, color=self.parse_rgba_color(qq_marker_color), s=qq_marker_size)
+        plt.title(
+            f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION\nRegression: {linear_regression.intercept:.4f} + x * {linear_regression.slope:.4f} • r = {linear_regression.rvalue:.4f}"
+        )
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
 
 if __name__ == "__main__":
 
     path = "../../datasets_test/continuous/data_1000/data_alpha.txt"
     # path = "../datasets_test/discrete/book2.txt"
     # path = "../datasets_test/continuous/data_1000/data_beta.txt"
```

### Comparing `phitter-0.0.4/phitter/discrete/__init__.py` & `phitter-0.0.5/phitter/discrete/__init__.py`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/__init__.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/bernoulli.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/bernoulli.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,20 @@
     Bernoulli distribution
     Parameters BERNOULLI distribution: {"p": *}
     https://phitter.io/distributions/discrete/bernoulli
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
         """
-        Initializes the BERNOULLI distribution by either providing a Continuous Measures instance [CONTINUOUS_MEASURES] or a dictionary with the distribution's parameters.
+        Initializes the BERNOULLI distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
         The BERNOULLI distribution parameters are: {"p": *}.
+        https://phitter.io/distributions/discrete/bernoulli
         """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -141,15 +142,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"p": *}
         """
         p = discrete_measures.mean
         parameters = {"p": p}
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/binomial.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/binomial.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,21 @@
     """
     Binomial distribution
     Parameters BINOMIAL distribution: {"n": *, "p": *}
     https://phitter.io/distributions/discrete/binomial
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the BINOMIAL distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The BINOMIAL distribution parameters are: {"n": *, "p": *}.
+        https://phitter.io/distributions/continuous/binomial
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -141,15 +146,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"n": *, "p": *}
         """
         p = 1 - discrete_measures.variance / discrete_measures.mean
         n = int(round(discrete_measures.mean / p, 0))
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/geometric.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/geometric.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,21 @@
     """
     Geometric distribution
     Parameters GEOMETRIC distribution: {"p": *}
     https://phitter.io/distributions/discrete/geometric
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the GEOMETRIC distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The GEOMETRIC distribution parameters are: {"p": *}.
+        https://phitter.io/distributions/continuous/geometric
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -139,15 +144,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"p": *}
         """
         p = 1 / discrete_measures.mean
         parameters = {"p": p}
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/hypergeometric.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/hypergeometric.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,21 @@
     """
     Hypergeometric_distribution
     Parameters HYPERGEOMETRIC distribution: {"N": *, "K": *, "n": *}
     https://phitter.io/distributions/discrete/hypergeometric
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the HYPERGEOMETRIC distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The HYPERGEOMETRIC distribution parameters are: {"N": *, "K": *, "n": *}.
+        https://phitter.io/distributions/continuous/hypergeometric
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -146,15 +151,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"N": *, "K": *, "n": *}
         """
 
         def equations(initial_solution: tuple[float], discrete_measures) -> tuple[float]:
@@ -173,18 +178,18 @@
             eq2 = parametric_variance - discrete_measures.variance
             # eq3 = parametric_skewness - discrete_measures.skewness
             # eq3 = parametric_kurtosis  - discrete_measures.kurtosis
             eq3 = parametric_mode - discrete_measures.mode
 
             return (eq1, eq2, eq3)
 
-        bnds = ((discrete_measures.max, discrete_measures.max, 1), (numpy.inf, numpy.inf, numpy.inf))
+        bounds = ((discrete_measures.max, discrete_measures.max, 1), (numpy.inf, numpy.inf, numpy.inf))
         x0 = (discrete_measures.max * 5, discrete_measures.max * 3, discrete_measures.max)
         args = [discrete_measures]
-        solution = scipy.optimize.least_squares(equations, x0, bounds=bnds, args=args)
+        solution = scipy.optimize.least_squares(equations, x0=x0, bounds=bounds, args=args)
         parameters = {"N": round(solution.x[0]), "K": round(solution.x[1]), "n": round(solution.x[2])}
 
         return parameters
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/logarithmic.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/logarithmic.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,21 @@
     """
     Logarithmic distribution
     Parameters LOGARITHMIC distribution: {"p": *}
     https://phitter.io/distributions/discrete/logarithmic
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the LOGARITHMIC distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The LOGARITHMIC distribution parameters are: {"p": *}.
+        https://phitter.io/distributions/continuous/logarithmic
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -144,15 +149,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"p": *}
         """
 
         def equations(initial_solution: tuple[float], discrete_measures) -> tuple[float]:
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/negative_binomial.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/negative_binomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,21 @@
     """
     Negative binomial distribution
     Parameters NEGATIVE_BINOMIAL distribution: {"r": *, "p": *}
     https://phitter.io/distributions/discrete/negative_binomial
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the NEGATIVE_BINOMIAL distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The NEGATIVE_BINOMIAL distribution parameters are: {"r": *, "p": *}.
+        https://phitter.io/distributions/continuous/negative_binomial
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -142,15 +147,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"r": *, "p": *}
         """
         p = discrete_measures.mean / discrete_measures.variance
         r = round(discrete_measures.mean * p / (1 - p))
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_distributions/poisson.py` & `phitter-0.0.5/phitter/discrete/discrete_distributions/poisson.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,21 @@
     """
     Poisson distribution
     Parameters POISSON distribution: {"lambda": *}
     https://phitter.io/distributions/discrete/poisson
     """
 
     def __init__(self, discrete_measures=None, parameters: dict[str, int | float] = None, init_parameters_examples=False):
+        """
+        Initializes the POISSON distribution by either providing a Discrete Measures instance [DISCRETE_MEASURES] or a dictionary with the distribution's parameters.
+        The POISSON distribution parameters are: {"lambda": *}.
+        https://phitter.io/distributions/continuous/poisson
+        """
         if discrete_measures is None and parameters is None and init_parameters_examples == False:
-            raise Exception("You must initialize the distribution by either providing the Continuous Measures [CONTINUOUS_MEASURES] instance or a dictionary of the distribution's parameters.")
+            raise Exception("You must initialize the distribution by either providing the Discrete Measures [DISCRETE_MEASURES] instance or a dictionary of the distribution's parameters.")
         if discrete_measures != None:
             self.parameters = self.get_parameters(discrete_measures)
         if parameters != None:
             self.parameters = parameters
         if init_parameters_examples:
             self.parameters = self.parameters_example
 
@@ -138,15 +143,15 @@
         """
         Calculate proper parameters of the distribution from sample discrete_measures.
         The parameters are calculated by formula.
 
         Parameters
         ==========
         discrete_measures: MEASUREMESTS
-            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, length, num_bins, data
+            attributes: mean, std, variance, skewness, kurtosis, median, mode, min, max, size, num_bins, data
 
         Returns
         =======
         parameters: {"lambda": *}
         """
         lambda_ = discrete_measures.mean
         parameters = {"lambda": lambda_}
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_measures/discrete_measures.py` & `phitter-0.0.5/phitter/discrete/discrete_measures/discrete_measures.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 
 
 class DISCRETE_MEASURES:
     def __init__(
         self,
         data: list[int],
         confidence_level: float = 0.95,
+        subsample_estimation_size: int | None = None,
     ):
         self.data = numpy.sort(data)
-        self.length = len(data)
-        self.min = min(data)
-        self.max = max(data)
+        self.size = self.data.size
+        self.data_to_fit = self.data if subsample_estimation_size == None else numpy.random.choice(self.data, size=min(self.size, subsample_estimation_size), replace=False)
+        self.min = self.data[0]
+        self.max = self.data[-1]
         self.mean = numpy.mean(data)
         self.variance = numpy.var(data, ddof=1)
         self.std = numpy.std(data, ddof=1)
         self.skewness = scipy.stats.moment(data, 3) / pow(self.std, 3)
         self.kurtosis = scipy.stats.moment(data, 4) / pow(self.std, 4)
         self.median = int(numpy.median(self.data))
         self.mode = int(scipy.stats.mode(data, keepdims=True)[0][0])
         self.domain = numpy.arange(self.min, self.max + 1)
         self.absolutes_frequencies, _ = numpy.histogram(self.data, bins=numpy.arange(self.min, self.max + 2) - 0.5, density=False)
         self.densities_frequencies, _ = numpy.histogram(self.data, bins=numpy.arange(self.min, self.max + 2) - 0.5, density=True)
-        self.idx_ks = numpy.concatenate([numpy.where(self.data[:-1] != self.data[1:])[0], [self.length - 1]])
-        self.Sn_ks = (numpy.arange(self.length) + 1) / self.length
+        self.idx_ks = numpy.concatenate([numpy.where(self.data[:-1] != self.data[1:])[0], [self.size - 1]])
+        self.Sn_ks = (numpy.arange(self.size) + 1) / self.size
         self.confidence_level = confidence_level
-        self.critical_value_ks = scipy.stats.kstwo.ppf(self.confidence_level, self.length)
+        self.critical_value_ks = scipy.stats.kstwo.ppf(self.confidence_level, self.size)
         self.ecdf_frequencies = numpy.cumsum(self.densities_frequencies)
-        self.qq_arr = (numpy.arange(1, self.length + 1) - 0.5) / self.length
+        self.qq_arr = (numpy.arange(1, self.size + 1) - 0.5) / self.size
 
     def __str__(self) -> str:
-        return str({"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
+        return str({"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
 
     def __repr__(self) -> str:
-        return str({"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
+        return str({"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode})
 
     def get_dict(self) -> str:
-        return {"length": self.length, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode}
+        return {"size": self.size, "mean": self.mean, "variance": self.variance, "skewness": self.skewness, "kurtosis": self.kurtosis, "median": self.median, "mode": self.mode}
 
     def critical_value_chi2(self, freedom_degrees):
         return scipy.stats.chi2.ppf(self.confidence_level, freedom_degrees)
 
 
 if __name__ == "__main__":
     ## Import function to get discrete_measures
@@ -53,15 +55,15 @@
 
     ## Distribution class
     path = "../discrete_distributions_sample/sample_geometric.txt"
     data = get_data(path)
 
     discrete_measures = DISCRETE_MEASURES(data)
 
-    print("Length: ", discrete_measures.length)
+    print("size: ", discrete_measures.size)
     print("Min: ", discrete_measures.min)
     print("Max: ", discrete_measures.max)
     print("Mean: ", discrete_measures.mean)
     print("Variance: ", discrete_measures.variance)
     print("Skewness: ", discrete_measures.skewness)
     print("Kurtosis: ", discrete_measures.kurtosis)
     print("Median: ", discrete_measures.median)
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_statistical_tests/discrete_test_chi_square.py` & `phitter-0.0.5/phitter/discrete/discrete_statistical_tests/discrete_test_chi_square.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             with the same degrees of freedom as for the critical value calculation.
         4. rejected(bool):
             decision if the null hypothesis is rejected. If it is false, it can be
             considered that the sample is distributed according to the probability
             distribution. If it's true, no.
     """
     ## Parameters and preparations
-    N = discrete_measures.length
+    N = discrete_measures.size
     freedom_degrees = max(len(discrete_measures.domain) - 1 - distribution.num_parameters, 1)
 
     ## Calculation of errors
     expected_values = numpy.ceil(N * (distribution.pmf(discrete_measures.domain)))
     errors = ((discrete_measures.absolutes_frequencies - expected_values) ** 2) / expected_values
 
     ## Calculation of indicators
```

### Comparing `phitter-0.0.4/phitter/discrete/discrete_statistical_tests/discrete_test_kolmogorov_smirnov.py` & `phitter-0.0.5/phitter/discrete/discrete_statistical_tests/discrete_test_kolmogorov_smirnov.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             whit size of sample N as parameter.
         4. rejected(bool):
             decision if the null hypothesis is rejected. If it is false, it can be
             considered that the sample is distributed according to the probability
             distribution. If it's true, no.
     """
     ## Parameters and preparations
-    N = discrete_measures.length
+    N = discrete_measures.size
 
     ## Calculation of errors
     Fn = distribution.cdf(discrete_measures.data)
     errors = numpy.abs(discrete_measures.Sn_ks[discrete_measures.idx_ks] - Fn[discrete_measures.idx_ks])
 
     ## Calculation of indicators
     statistic_ks = numpy.max(errors)
```

### Comparing `phitter-0.0.4/phitter/discrete/phitter_discrete.py` & `phitter-0.0.5/phitter/discrete/phitter_discrete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 import concurrent.futures
+import random
+import re
 import typing
-import sys
 
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy
 import plotly.express as px
 import plotly.graph_objects as go
 import scipy.stats
 
 
 class PHITTER_DISCRETE:
     def __init__(
         self,
         data: list[int | float] | numpy.ndarray,
         confidence_level=0.95,
         minimum_sse=numpy.inf,
+        subsample_estimation_size: int | None = None,
         distributions_to_fit: list[str] | typing.Literal["all"] = "all",
+        exclude_distributions: list[str] | typing.Literal["any"] = "any",
     ):
-        if distributions_to_fit != "all":
+        if distributions_to_fit != "all" and exclude_distributions != "any":
+            raise Exception(f"Specify either distributions_to_fit or exclude_distributions, not both.")
+
+        if distributions_to_fit == "all" and exclude_distributions == "any":
+            self.distributions_to_fit = list(ALL_DISCRETE_DISTRIBUTIONS.keys())
+
+        if distributions_to_fit != "all" and exclude_distributions == "any":
             not_distributions_ids = [dist for dist in distributions_to_fit if dist not in ALL_DISCRETE_DISTRIBUTIONS.keys()]
             if len(not_distributions_ids) > 0:
-                raise Exception(f"{not_distributions_ids} not founded in cdiscrete disributions")
+                raise Exception(f"{not_distributions_ids} not founded in discrete disributions")
+            self.distributions_to_fit = distributions_to_fit
 
-        self.data = data
-        self.discrete_measures = DISCRETE_MEASURES(self.data)
-        self.confidence_level = confidence_level
+        if distributions_to_fit == "all" and exclude_distributions != "any":
+            not_distributions_ids = [dist for dist in exclude_distributions if dist not in ALL_DISCRETE_DISTRIBUTIONS.keys()]
+            if len(not_distributions_ids) > 0:
+                raise Exception(f"{not_distributions_ids} not founded in discrete disributions")
+            self.distributions_to_fit = [dist for dist in ALL_DISCRETE_DISTRIBUTIONS.keys() if dist not in exclude_distributions]
+
+        self.discrete_measures = DISCRETE_MEASURES(
+            data=data,
+            confidence_level=confidence_level,
+            subsample_estimation_size=subsample_estimation_size,
+        )
         self.minimum_sse = minimum_sse
         self.distribution_results = {}
         self.none_results = {"test_statistic": None, "critical_value": None, "p_value": None, "rejected": None}
         self.distributions_to_fit = list(ALL_DISCRETE_DISTRIBUTIONS.keys()) if distributions_to_fit == "all" else distributions_to_fit
         self.sorted_distributions_sse = None
         self.not_rejected_distributions = None
         self.distribution_instances = None
@@ -88,24 +108,30 @@
             processing_results = list(executor.map(self.process_distribution, self.distributions_to_fit))
 
         processing_results = [r for r in processing_results if r is not None]
         self.sorted_distributions_sse = {distribution: results for distribution, results, _ in sorted(processing_results, key=lambda x: (-x[1]["n_test_passed"], x[1]["sse"]))}
         self.not_rejected_distributions = {distribution: results for distribution, results in self.sorted_distributions_sse.items() if results["n_test_passed"] > 0}
         self.distribution_instances = {distribution: instance for distribution, _, instance in processing_results}
 
-    def plot_histogram(
+    def parse_rgba_color(self, rgba_string):
+        rgba = re.match(r"rgba\((\d+),(\d+),(\d+),(\d*(?:\.\d+)?)\)", rgba_string)
+        r, g, b, a = map(float, rgba.groups())
+        return (r / 255, g / 255, b / 255, a)
+
+    def plot_histogram_plotly(
         self,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
+        plot_renderer: str | None,
     ):
         domain = self.discrete_measures.domain
         densities_frequencies = self.discrete_measures.densities_frequencies
 
         fig = go.Figure()
         fig.add_trace(go.Bar(x=domain, y=densities_frequencies, marker_color=plot_bar_color, name="Data", showlegend=True))
         fig.update_layout(
@@ -115,28 +141,54 @@
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10), title_font_size=11),
             bargap=plot_bargap,
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_histogram_matplotlib(
+        self,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None = None,
+    ):
+        matplotlib.style.use("ggplot")
+        domain = self.discrete_measures.domain
+        densities_frequencies = self.discrete_measures.densities_frequencies
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        # plt.hist(self.discrete_measures.data, density=True, label="Data", bins=self.discrete_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
+        plt.bar(domain, densities_frequencies, label="Data", color=self.parse_rgba_color(plot_bar_color))
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
-    def plot_histogram_distributions_pmf(
+    def plot_histogram_distributions_pmf_plotly(
         self,
         n_distributions: int,
         n_distributions_visible: int,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
+        plot_renderer: str | None,
     ):
         domain = self.discrete_measures.domain
         densities_frequencies = self.discrete_measures.densities_frequencies
 
         fig = go.Figure()
         fig.add_trace(go.Bar(x=domain, y=densities_frequencies, marker_color=plot_bar_color, name="Data", showlegend=False))
 
@@ -162,29 +214,68 @@
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
             bargap=plot_bargap,
         )
 
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def plot_histogram_distributions_pmf_matplotlib(
+        self,
+        n_distributions: int,
+        n_distributions_visible: int,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        domain = self.discrete_measures.domain
+        densities_frequencies = self.discrete_measures.densities_frequencies
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        # plt.hist(self.discrete_measures.data, density=True, bins=self.discrete_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
+        plt.bar(domain, densities_frequencies, color=self.parse_rgba_color(plot_bar_color))
+
+        for idx, (distribution_name, result) in enumerate(list(self.sorted_distributions_sse.items())[:n_distributions]):
+            y_plot = self.distribution_instances[distribution_name].pmf(domain)
+            distribution_sse = result["sse"]
+            is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+            scatter_name = f"{idx+1:02d}. {distribution_name}: {distribution_sse:.4E}{is_rejected}"
+            try:
+                plt.plot(domain, y_plot, label=scatter_name, color=(random.uniform(0, 1), random.uniform(0, 1), random.uniform(0, 1)), marker=".")
+            except Exception:
+                plt.plot(domain, numpy.zeros(len(domain)), label=scatter_name, color=(random.uniform(0, 1), random.uniform(0, 1), random.uniform(0, 1)), marker=".")
+
+        plt.title(f"{plot_title} - PMF DISTRIBUTIONS")
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
-    def plot_distribution_pmf(
+    def plot_distribution_pmf_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
         plot_line_color: str,
         plot_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         domain = self.discrete_measures.domain
         densities_frequencies = self.discrete_measures.densities_frequencies
 
@@ -212,26 +303,68 @@
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
             bargap=plot_bargap,
         )
 
-        fig.show()
+        fig.show(renderer=plot_renderer)
 
-    def plot_ecdf(
+    def plot_distribution_pmf_matplotlib(
         self,
+        distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_bar_color: str,
         plot_bargap: float,
+        plot_line_color: str,
+        plot_line_width: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        domain = self.discrete_measures.domain
+        densities_frequencies = self.discrete_measures.densities_frequencies
+
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not founded")
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        # plt.hist(self.discrete_measures.data, density=True, label="Data", bins=self.discrete_measures.num_bins, ec="white", color=self.parse_rgba_color(plot_bar_color))
+        plt.bar(domain, densities_frequencies, label="Data", color=self.parse_rgba_color(plot_bar_color))
+
+        y_plot = self.distribution_instances[distribution_name].pmf(domain)
+        distribution_sse = self.sorted_distributions_sse[distribution_name]["sse"]
+        is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+        scatter_name = f"{distribution_name}: {distribution_sse:.4E}{is_rejected}"
+        try:
+            plt.plot(domain, y_plot, label=scatter_name, color=self.parse_rgba_color(plot_line_color), linewidth=plot_line_width, marker="o")
+        except Exception:
+            plt.plot(domain, numpy.zeros(len(domain)), label=scatter_name, color=self.parse_rgba_color(plot_line_color), linewidth=plot_line_width, marker="o")
+
+        plt.title(f"{plot_title} - PMF {distribution_name.upper().replace('_', ' ')} DISTRIBUTION")
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def plot_ecdf_plotly(
+        self,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None,
     ):
         domain = self.discrete_measures.domain
         ecdf_frequencies = self.discrete_measures.ecdf_frequencies
 
         fig = go.Figure()
         fig.add_trace(go.Bar(x=domain, y=ecdf_frequencies, marker_color=plot_bar_color, name="Empirical Distribution", showlegend=True))
         fig.update_layout(
@@ -243,29 +376,60 @@
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
             bargap=plot_bargap,
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
 
-    def plot_ecdf_distribution(
+    def plot_ecdf_matplotlib(
+        self,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_bar_color: str,
+        plot_bargap: float,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+
+        matplotlib.style.use("ggplot")
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.hist(
+            self.discrete_measures.data,
+            density=True,
+            cumulative=True,
+            label="Data",
+            ec="white",
+            color=self.parse_rgba_color(plot_bar_color),
+        )
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def plot_ecdf_distribution_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         plot_empirical_bar_color: str,
         plot_empirical_bargap: float,
         plot_distribution_line_color: str,
         plot_distribution_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         domain = self.discrete_measures.domain
         ecdf_frequencies = self.discrete_measures.ecdf_frequencies
 
@@ -297,28 +461,79 @@
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
             bargap=plot_empirical_bargap,
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
 
-    def qq_plot(
+    def plot_ecdf_distribution_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        plot_empirical_bar_color: str,
+        plot_empirical_bargap: float,
+        plot_distribution_line_color: str,
+        plot_distribution_line_width: int,
+        plot_renderer: str | None,
+    ):
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not founded")
+
+        matplotlib.style.use("ggplot")
+
+        domain = self.discrete_measures.domain
+        ecdf_frequencies = self.discrete_measures.ecdf_frequencies
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        # plt.hist(
+        #     self.discrete_measures.data,
+        #     density=True,
+        #     cumulative=True,
+        #     label="Data",
+        #     ec="white",
+        #     color=self.parse_rgba_color(plot_empirical_bar_color),
+        # )
+        plt.bar(domain, ecdf_frequencies, label="Data", color=self.parse_rgba_color(plot_empirical_bar_color))
+
+        domain = self.discrete_measures.domain
+        y_plot = self.distribution_instances[distribution_name].cdf(domain)
+        distribution_sse = self.sorted_distributions_sse[distribution_name]["sse"]
+        is_rejected = "✓" if distribution_name in self.not_rejected_distributions else ""
+        scatter_name = f"{distribution_name}: {distribution_sse:.4E}{is_rejected}"
+        try:
+            plt.plot(domain, y_plot, label=scatter_name, color=self.parse_rgba_color(plot_distribution_line_color), linewidth=plot_distribution_line_width, marker=".")
+        except Exception:
+            plt.plot(domain, numpy.zeros(len(domain)), label=scatter_name, color=self.parse_rgba_color(plot_distribution_line_color), linewidth=plot_distribution_line_width)
+
+        plt.title(plot_title)
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def qq_plot_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         qq_marker_name: str,
         qq_marker_color: str,
         qq_marker_size: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         x = self.distribution_instances[distribution_name].ppf(self.discrete_measures.qq_arr)
         y = self.discrete_measures.data
 
@@ -332,31 +547,61 @@
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
 
-    def qq_plot_regression(
+    def qq_plot_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        qq_marker_name: str,
+        qq_marker_color: str,
+        qq_marker_size: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not found")
+
+        x = self.distribution_instances[distribution_name].ppf(self.discrete_measures.qq_arr)
+        y = self.discrete_measures.data
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.scatter(x, y, label=qq_marker_name, color=self.parse_rgba_color(qq_marker_color), s=qq_marker_size)
+        plt.title(f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION")
+        plt.xlabel(plot_xaxis_title)
+        plt.ylabel(plot_yaxis_title)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
+
+    def qq_plot_regression_plotly(
         self,
         distribution_name: str,
         plot_title: str,
         plot_xaxis_title: str,
         plot_yaxis_title: str,
         plot_legend_title: str,
         plot_height: int,
         plot_width: int,
         qq_marker_name: str,
         qq_marker_color: str,
         qq_marker_size: int,
         regression_line_name: str,
         regression_line_color: str,
         regression_line_width: int,
+        plot_renderer: str | None,
     ):
         if distribution_name not in self.distribution_instances:
             raise Exception(f"{distribution_name} distribution not founded")
 
         x = self.distribution_instances[distribution_name].ppf(self.discrete_measures.qq_arr)
         y = self.discrete_measures.data
 
@@ -365,40 +610,76 @@
 
         fig = go.Figure()
         fig.add_trace(go.Scatter(x=x, y=y_reg, mode="lines", name=regression_line_name, line=dict(color=regression_line_color, width=regression_line_width)))
         fig.add_trace(go.Scatter(x=x, y=y, mode="markers", name=qq_marker_name, marker=dict(color=qq_marker_color, size=qq_marker_size)))
         fig.update_layout(
             height=plot_height,
             width=plot_width,
-            title=f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION <br><br><sup>Regression: {linear_regression.intercept:.4g} + x * {linear_regression.slope:.4g} • r = {linear_regression.rvalue:.4g}</sup>",
+            title=f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION <br><br><sup>Regression: {linear_regression.intercept:.4f} + x * {linear_regression.slope:.4f} • r = {linear_regression.rvalue:.4f}</sup>",
             xaxis_title=plot_xaxis_title,
             yaxis_title=plot_yaxis_title,
             legend_title=plot_legend_title,
             template="ggplot2",
             xaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             yaxis=dict(title_font_size=12, tickfont=dict(size=10)),
             legend=dict(orientation="v", yanchor="auto", y=1, xanchor="left", font=dict(size=10)),
         )
-        fig.show()
+        fig.show(renderer=plot_renderer)
+
+    def qq_plot_regression_matplotlib(
+        self,
+        distribution_name: str,
+        plot_title: str,
+        plot_xaxis_title: str,
+        plot_yaxis_title: str,
+        plot_legend_title: str,
+        plot_height: int,
+        plot_width: int,
+        qq_marker_name: str,
+        qq_marker_color: str,
+        qq_marker_size: int,
+        regression_line_name: str,
+        regression_line_color: str,
+        regression_line_width: int,
+        plot_renderer: str | None,
+    ):
+        matplotlib.style.use("ggplot")
+        if distribution_name not in self.distribution_instances:
+            raise Exception(f"{distribution_name} distribution not found")
+
+        x = self.distribution_instances[distribution_name].ppf(self.discrete_measures.qq_arr)
+        y = self.discrete_measures.data
+
+        linear_regression = scipy.stats.linregress(x, y)
+        y_reg = linear_regression.intercept + x * linear_regression.slope
+
+        plt.figure(figsize=(plot_width / 100, plot_height / 100))
+        plt.plot(x, y_reg, label=regression_line_name, color=self.parse_rgba_color(regression_line_color), linewidth=regression_line_width)
+        plt.scatter(x, y, label=qq_marker_name, color=self.parse_rgba_color(qq_marker_color), s=qq_marker_size)
+        plt.title(
+            f"{plot_title} {distribution_name.upper().replace('_', ' ')} DISTRIBUTION\nRegression: {linear_regression.intercept:.4f} + x * {linear_regression.slope:.4f} • r = {linear_regression.rvalue:.4f}"
+        )
+        plt.xlabel(plot_xaxis_title, fontsize=10)
+        plt.ylabel(plot_yaxis_title, fontsize=10)
+        plt.legend(title=plot_legend_title, fontsize=8, bbox_to_anchor=(1.01, 1.01), loc="upper left")
+        plt.show()
 
 
 if __name__ == "__main__":
     from discrete_distributions import ALL_DISCRETE_DISTRIBUTIONS
     from discrete_measures import DISCRETE_MEASURES
-    from discrete_statistical_tests import evaluate_discrete_test_chi_square
-    from discrete_statistical_tests import evaluate_discrete_test_kolmogorov_smirnov
+    from discrete_statistical_tests import evaluate_discrete_test_chi_square, evaluate_discrete_test_kolmogorov_smirnov
 
     path = "../../datasets_test/discrete/sample_binomial.txt"
     sample_distribution_file = open(path, "r", encoding="utf-8-sig")
     data = [float(x.replace(",", ".")) for x in sample_distribution_file.read().splitlines()]
     sample_distribution_file.close()
 
     phitter_discrete = PHITTER_DISCRETE(data)
     phitter_discrete.fit()
 
     for distribution, results in phitter_discrete.sorted_distributions_sse.items():
         print(f"Distribution: {distribution}, SSE: {results['sse']}, Aprobados: {results['n_test_passed']}")
 else:
     from phitter.discrete.discrete_distributions import ALL_DISCRETE_DISTRIBUTIONS
     from phitter.discrete.discrete_measures import DISCRETE_MEASURES
-    from phitter.discrete.discrete_statistical_tests import evaluate_discrete_test_chi_square
-    from phitter.discrete.discrete_statistical_tests import evaluate_discrete_test_kolmogorov_smirnov
+    from phitter.discrete.discrete_statistical_tests import evaluate_discrete_test_chi_square, evaluate_discrete_test_kolmogorov_smirnov
```

### Comparing `phitter-0.0.4/phitter.egg-info/SOURCES.txt` & `phitter-0.0.5/phitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phitter-0.0.4/pyproject.toml` & `phitter-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phitter"
-version = "0.0.4"
+version = "0.0.5"
 description = "Find the best probability distribution for your dataset"
 authors = [{name = "Sebastián José Herrera Monterrosa", email = "phitter.email@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["scientific", "engineering", "mathematics", "artificial intelligence", "software development", "python modules"]
 classifiers = [
@@ -30,15 +30,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "scipy>=1.1.0",
-    "plotly>=5.14.0"
+    "plotly>=5.14.0",
+    "kaleido>=0.2.1",
+    "matplotlib>=3.3"
 ]
 
 [project.urls]
 Homepage = "https://phitter.io"
 Documentation = "https://github.com/phitterio/phitter-kernel"
 Repository = "https://github.com/phitterio/phitter-kernel"
```

