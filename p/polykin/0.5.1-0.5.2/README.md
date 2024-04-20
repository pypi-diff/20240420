# Comparing `tmp/polykin-0.5.1.tar.gz` & `tmp/polykin-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polykin-0.5.1.tar", max compression
+gzip compressed data, was "polykin-0.5.2.tar", max compression
```

## Comparing `polykin-0.5.1.tar` & `polykin-0.5.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1066 2024-04-14 21:31:23.594301 polykin-0.5.1/LICENSE
--rw-r--r--   0        0        0     3022 2024-04-14 21:31:23.594301 polykin-0.5.1/README.md
--rw-r--r--   0        0        0     1801 2024-04-14 21:31:23.614301 polykin-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      701 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/__init__.py
--rw-r--r--   0        0        0      366 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/__init__.py
--rw-r--r--   0        0        0     4533 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/binary.py
--rw-r--r--   0        0        0     6932 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/copodataset.py
--rw-r--r--   0        0        0    12850 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/fitting.py
--rw-r--r--   0        0        0    19779 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/multicomponent.py
--rw-r--r--   0        0        0    17038 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/penultimate.py
--rw-r--r--   0        0        0    24303 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/copolymerization/terminal.py
--rw-r--r--   0        0        0      362 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/__init__.py
--rw-r--r--   0        0        0    11409 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/analyticaldistributions.py
--rw-r--r--   0        0        0    27752 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/base.py
--rw-r--r--   0        0        0     7334 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/datadistribution.py
--rw-r--r--   0        0        0    30255 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/distributions/sampledata.py
--rw-r--r--   0        0        0      335 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/__init__.py
--rw-r--r--   0        0        0     9460 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/arrhenius.py
--rw-r--r--   0        0        0      846 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/base.py
--rw-r--r--   0        0        0     4078 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/cldpropagation.py
--rw-r--r--   0        0        0     4936 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/cldtermination.py
--rw-r--r--   0        0        0     3704 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/kinetics/eyring.py
--rw-r--r--   0        0        0      198 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/derivatives.py
--rw-r--r--   0        0        0     9805 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/math/jcr.py
--rw-r--r--   0        0        0      281 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/__init__.py
--rw-r--r--   0        0        0      284 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/liquid.py
--rw-r--r--   0        0        0     3759 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/vapor.py
--rw-r--r--   0        0        0    11866 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/diffusion/vrentasduda.py
--rw-r--r--   0        0        0      323 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/__init__.py
--rw-r--r--   0        0        0    10887 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/base.py
--rw-r--r--   0        0        0    14174 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/dippr.py
--rw-r--r--   0        0        0     6429 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/vapor_pressure.py
--rw-r--r--   0        0        0     3070 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/equations/viscosity.py
--rw-r--r--   0        0        0     4274 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/mixing_rules.py
--rw-r--r--   0        0        0     3348 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
--rw-r--r--   0        0        0     3722 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
--rw-r--r--   0        0        0     3298 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
--rw-r--r--   0        0        0     2954 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
--rw-r--r--   0        0        0      213 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/__init__.py
--rw-r--r--   0        0        0     6555 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/base.py
--rw-r--r--   0        0        0    10277 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/eos.py
--rw-r--r--   0        0        0     5566 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/pvt_polymer/tait.py
--rw-r--r--   0        0        0      272 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/__init__.py
--rw-r--r--   0        0        0     2159 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/liquid.py
--rw-r--r--   0        0        0     7252 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/thermal_conductivity/vapor.py
--rw-r--r--   0        0        0     7619 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/vaporization_enthalpy.py
--rw-r--r--   0        0        0      247 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/viscosity/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-14 21:31:23.614301 polykin-0.5.1/src/polykin/properties/viscosity/liquid.py
--rw-r--r--   0        0        0    12768 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/properties/viscosity/vapor.py
--rw-r--r--   0        0        0      215 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/stepgrowth/__init__.py
--rw-r--r--   0        0        0    34496 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/stepgrowth/solutions.py
--rw-r--r--   0        0        0      195 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/__init__.py
--rw-r--r--   0        0        0      287 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/__init__.py
--rw-r--r--   0        0        0    12659 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/base.py
--rw-r--r--   0        0        0    12655 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/floryhuggins.py
--rw-r--r--   0        0        0      886 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/ideal.py
--rw-r--r--   0        0        0     7621 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/nrtl.py
--rw-r--r--   0        0        0     9363 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/polynrtl.py
--rw-r--r--   0        0        0     7513 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/uniquac.py
--rw-r--r--   0        0        0     4953 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/acm/wilson.py
--rw-r--r--   0        0        0      260 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/__init__.py
--rw-r--r--   0        0        0     6544 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/base.py
--rw-r--r--   0        0        0    15285 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/cubic.py
--rw-r--r--   0        0        0     1976 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/idealgas.py
--rw-r--r--   0        0        0     9579 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/thermo/eos/virial.py
--rw-r--r--   0        0        0       86 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/__init__.py
--rw-r--r--   0        0        0      356 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/exceptions.py
--rw-r--r--   0        0        0     3082 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/math.py
--rw-r--r--   0        0        0     9976 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/tools.py
--rw-r--r--   0        0        0     1088 2024-04-14 21:31:23.618301 polykin-0.5.1/src/polykin/utils/types.py
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 polykin-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-20 10:01:01.127110 polykin-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3034 2024-04-20 10:01:01.127110 polykin-0.5.2/README.md
+-rw-r--r--   0        0        0     1801 2024-04-20 10:01:01.147110 polykin-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      701 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/__init__.py
+-rw-r--r--   0        0        0     7309 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/binary.py
+-rw-r--r--   0        0        0     6932 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/copodataset.py
+-rw-r--r--   0        0        0    12812 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/fitting.py
+-rw-r--r--   0        0        0    19738 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/multicomponent.py
+-rw-r--r--   0        0        0    17038 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/penultimate.py
+-rw-r--r--   0        0        0    24303 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/copolymerization/terminal.py
+-rw-r--r--   0        0        0      362 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/distributions/__init__.py
+-rw-r--r--   0        0        0    11409 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/distributions/analyticaldistributions.py
+-rw-r--r--   0        0        0    27752 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/distributions/base.py
+-rw-r--r--   0        0        0     7334 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/distributions/datadistribution.py
+-rw-r--r--   0        0        0    30255 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/distributions/sampledata.py
+-rw-r--r--   0        0        0      335 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/__init__.py
+-rw-r--r--   0        0        0     9448 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/arrhenius.py
+-rw-r--r--   0        0        0      846 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/base.py
+-rw-r--r--   0        0        0     4078 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/cldpropagation.py
+-rw-r--r--   0        0        0     4936 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/cldtermination.py
+-rw-r--r--   0        0        0     3692 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/kinetics/eyring.py
+-rw-r--r--   0        0        0      198 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/math/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/math/derivatives.py
+-rw-r--r--   0        0        0     9776 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/math/jcr.py
+-rw-r--r--   0        0        0      281 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/diffusion/__init__.py
+-rw-r--r--   0        0        0     4645 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/diffusion/liquid.py
+-rw-r--r--   0        0        0     3759 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/diffusion/vapor.py
+-rw-r--r--   0        0        0    11866 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/diffusion/vrentasduda.py
+-rw-r--r--   0        0        0      323 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/equations/__init__.py
+-rw-r--r--   0        0        0    10887 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/equations/base.py
+-rw-r--r--   0        0        0    14174 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/equations/dippr.py
+-rw-r--r--   0        0        0     6410 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/equations/vapor_pressure.py
+-rw-r--r--   0        0        0     3070 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/equations/viscosity.py
+-rw-r--r--   0        0        0     4274 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/mixing_rules.py
+-rw-r--r--   0        0        0     3348 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
+-rw-r--r--   0        0        0     3722 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
+-rw-r--r--   0        0        0     3298 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
+-rw-r--r--   0        0        0     2954 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
+-rw-r--r--   0        0        0      213 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/__init__.py
+-rw-r--r--   0        0        0     6555 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/base.py
+-rw-r--r--   0        0        0    10277 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/eos.py
+-rw-r--r--   0        0        0     5566 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/pvt_polymer/tait.py
+-rw-r--r--   0        0        0      272 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/thermal_conductivity/__init__.py
+-rw-r--r--   0        0        0     2159 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/thermal_conductivity/liquid.py
+-rw-r--r--   0        0        0     7252 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/thermal_conductivity/vapor.py
+-rw-r--r--   0        0        0     7619 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/vaporization_enthalpy.py
+-rw-r--r--   0        0        0      247 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/viscosity/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-20 10:01:01.147110 polykin-0.5.2/src/polykin/properties/viscosity/liquid.py
+-rw-r--r--   0        0        0    12768 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/properties/viscosity/vapor.py
+-rw-r--r--   0        0        0      215 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/stepgrowth/__init__.py
+-rw-r--r--   0        0        0    34496 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/stepgrowth/solutions.py
+-rw-r--r--   0        0        0      195 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/__init__.py
+-rw-r--r--   0        0        0    12659 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/base.py
+-rw-r--r--   0        0        0    12628 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/floryhuggins.py
+-rw-r--r--   0        0        0      886 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/ideal.py
+-rw-r--r--   0        0        0     7598 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/nrtl.py
+-rw-r--r--   0        0        0     9363 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/polynrtl.py
+-rw-r--r--   0        0        0     7479 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/uniquac.py
+-rw-r--r--   0        0        0     4926 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/acm/wilson.py
+-rw-r--r--   0        0        0      260 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/eos/__init__.py
+-rw-r--r--   0        0        0     6544 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/eos/base.py
+-rw-r--r--   0        0        0    15285 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/eos/cubic.py
+-rw-r--r--   0        0        0     1976 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/eos/idealgas.py
+-rw-r--r--   0        0        0     9579 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/thermo/eos/virial.py
+-rw-r--r--   0        0        0       86 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/utils/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/utils/exceptions.py
+-rw-r--r--   0        0        0     3082 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/utils/math.py
+-rw-r--r--   0        0        0     9976 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/utils/tools.py
+-rw-r--r--   0        0        0     1088 2024-04-20 10:01:01.151110 polykin-0.5.2/src/polykin/utils/types.py
+-rw-r--r--   0        0        0     4143 1970-01-01 00:00:00.000000 polykin-0.5.2/PKG-INFO
```

### Comparing `polykin-0.5.1/LICENSE` & `polykin-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/README.md` & `polykin-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   - [x] UNIQUAC
   - [x] Wilson
 - Copolymerization
   - [x] Implicit penultimate model
   - [x] Penultimate model
   - [x] Terminal model
   - [x] Mayo-Lewis equation (binary, ternary and multicomponent)
-  - [x] Monomer dift equation (multicomponent)
+  - [x] Monomer drift equation (binary and multicomponent)
   - [ ] Fitting methods
 - Equations of state
   - [50%] Cubic (Redlich-Kwong, Soave, Peng-Robinson)
   - [x] Ideal gas
   - [ ] Sanchez-Lacombe
   - [x] Virial equation
 - [ ] Database
```

#### html2text {}

```diff
@@ -5,31 +5,32 @@
 Commit](https://img.shields.io/github/last-commit/HugoMVale/polykin)](https://
 img.shields.io/github/last-commit/HugoMVale/polykin) PolyKin is an open-source
 polymerization kinetics library for Python. It is still at an early development
 stage, but the following modules can already be used: - Activity coefficient
 models - [x] Ideal solution - [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL -
 [x] UNIQUAC - [x] Wilson - Copolymerization - [x] Implicit penultimate model -
 [x] Penultimate model - [x] Terminal model - [x] Mayo-Lewis equation (binary,
-ternary and multicomponent) - [x] Monomer dift equation (multicomponent) - [ ]
-Fitting methods - Equations of state - [50%] Cubic (Redlich-Kwong, Soave, Peng-
-Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe - [x] Virial equation - [ ]
-Database - Distributions - [x] Flory - [ ] Gold - [x] Log-normal - [x] Poison -
-[x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x] Eyring - [x] Propagation half-
-length - [x] Termination composite model - Math - [x] Joint confidence regions
-- [ ] Models - Physical property correlations - [x] Antoine - [x] DIPPR - [x]
-Wagner - [x] Yaws - Step-growth polymerization - [x] Analytical solutions for
-$M_n$ and $M_w$ - Transport properties (estimation methods, mixing rules, etc.)
-- Diffusivity - [x] Binary gas mixtures - [x] Binary liquid mixtures - [x]
-Binary polymer solutions - [ ] Multicomponent polymer solutions - Thermal
-conductivity - [x] Gases - [x] Liquids - [ ] Polymer solutions - Viscosity -
-[x] Gases - [x] Liquids - [ ] Polymer solutions ## Documentation Please refer
-to the package [homepage](https://hugomvale.github.io/polykin/). ## Tutorials
-The main features of PolyKin are explained and illustrated through a series of
-[tutorials](https://hugomvale.github.io/polykin/tutorials/) based on Jupyter
-[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
-which can be launched online via Binder.
+ternary and multicomponent) - [x] Monomer drift equation (binary and
+multicomponent) - [ ] Fitting methods - Equations of state - [50%] Cubic
+(Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe -
+[x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ] Gold - [x]
+Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x]
+Eyring - [x] Propagation half-length - [x] Termination composite model - Math -
+[x] Joint confidence regions - [ ] Models - Physical property correlations -
+[x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth polymerization -
+[x] Analytical solutions for $M_n$ and $M_w$ - Transport properties (estimation
+methods, mixing rules, etc.) - Diffusivity - [x] Binary gas mixtures - [x]
+Binary liquid mixtures - [x] Binary polymer solutions - [ ] Multicomponent
+polymer solutions - Thermal conductivity - [x] Gases - [x] Liquids - [ ]
+Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ] Polymer solutions
+## Documentation Please refer to the package [homepage](https://
+hugomvale.github.io/polykin/). ## Tutorials The main features of PolyKin are
+explained and illustrated through a series of [tutorials](https://
+hugomvale.github.io/polykin/tutorials/) based on Jupyter [notebooks](https://
+github.com/HugoMVale/polykin/tree/main/docs/tutorials), which can be launched
+online via Binder.
                            _[_M_W_D_ _o_f_ _a_ _p_o_l_y_m_e_r_ _b_l_e_n_d_]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

### Comparing `polykin-0.5.1/pyproject.toml` & `polykin-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polykin"
-version = "0.5.1"
+version = "0.5.2"
 description = "A polymerization kinetics library."
 authors = ["HugoMVale <57530119+HugoMVale@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hugomvale.github.io/polykin/"
 repository = "https://github.com/HugoMVale/polykin"
 documentation = "https://hugomvale.github.io/polykin/"
```

### Comparing `polykin-0.5.1/src/polykin/__init__.py` & `polykin-0.5.2/src/polykin/__init__.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/copolymerization/copodataset.py` & `polykin-0.5.2/src/polykin/copolymerization/copodataset.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/copolymerization/fitting.py` & `polykin-0.5.2/src/polykin/copolymerization/fitting.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,21 +175,21 @@
         the resolution of the JCR appears insufficient.
 
     Returns
     -------
     CopoFitResult
         Dataclass with all fit results.
 
-    !!! note annotate "See also"
-
-        * [`confidence_ellipse`](../math/confidence_ellipse.md): linear method
-        used to calculate the joint confidence region.
-        * [`confidence_region`](../math/confidence_region.md): exact method
-        used to calculate the joint confidence region.
-        * [`fit_Finemann_Ross`](fit_Finemann_Ross.md): alternative method.  
+    See also
+    --------
+    * [`confidence_ellipse`](../math/confidence_ellipse.md): linear method
+      used to calculate the joint confidence region.
+    * [`confidence_region`](../math/confidence_region.md): exact method
+      used to calculate the joint confidence region.
+    * [`fit_Finemann_Ross`](fit_Finemann_Ross.md): alternative method.  
 
     Examples
     --------
     >>> from polykin.copolymerization.fitting import fit_reactivity_ratios
     >>>
     >>> f1 = [0.186, 0.299, 0.527, 0.600, 0.700, 0.798]
     >>> F1 = [0.196, 0.279, 0.415, 0.473, 0.542, 0.634]
@@ -351,18 +351,18 @@
         Vector of instantaneous copolymer composition of M1, $F_1$.
 
     Returns
     -------
     tuple[float, float]
         Point estimates of the reactivity ratios $(r_1, r_2)$.
 
-    !!! note annotate "See also"
-
-        * [`fit_reactivity_ratios`](fit_reactivity_ratios.md): alternative
-        (recommended) method.  
+    See also
+    --------
+    * [`fit_reactivity_ratios`](fit_reactivity_ratios.md): alternative
+      (recommended) method.  
 
     Examples
     --------
     >>> from polykin.copolymerization.fitting import fit_Finemann_Ross
     >>>
     >>> f1 = [0.186, 0.299, 0.527, 0.600, 0.700, 0.798]
     >>> F1 = [0.196, 0.279, 0.415, 0.473, 0.542, 0.634]
```

### Comparing `polykin-0.5.1/src/polykin/copolymerization/multicomponent.py` & `polykin-0.5.2/src/polykin/copolymerization/multicomponent.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,20 +83,20 @@
         Reactivity ratio.
 
     Returns
     -------
     tuple[float | FloatArray, ...]
         Instantaneous terpolymer composition, $(F_1, F_2, F_3)$.
 
-    !!! note annotate "See also"
-
-        * [`inst_copolymer_binary`](inst_copolymer_binary.md):
-          specific method for binary systems.
-        * [`inst_copolymer_multi`](inst_copolymer_multi.md):
-          generic method for multicomponent systems.
+    See also
+    --------
+    * [`inst_copolymer_binary`](inst_copolymer_binary.md):
+      specific method for binary systems.
+    * [`inst_copolymer_multi`](inst_copolymer_multi.md):
+      generic method for multicomponent systems.
 
     Examples
     --------
     >>> from polykin.copolymerization import inst_copolymer_ternary
     >>>
     >>> F1, F2, F3 = inst_copolymer_ternary(f1=0.5, f2=0.3, r12=0.2, r21=2.3,
     ...                                     r13=3.0, r31=0.9, r23=0.4, r32=1.5)
@@ -156,46 +156,46 @@
     \vdots \\
     1
     \end{bmatrix} $$
 
     where $P_{ij}$ are the transition probabilitites, which can be computed
     from the instantaneous monomer composition and the reactivity matrix.
 
+    **References**
+
+    *   H. K. Frensdorff, R. Pariser; Copolymerization as a Markov Chain.
+        J. Chem. Phys. 1 November 1963; 39 (9): 2303-2309.
+
     Parameters
     ----------
-    f : FloatVectorLike | None
-        Vector (N) of instantaneous monomer compositions, $f_i$.
-    r : FloatSquareMatrix | None
-        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
-    P : FloatSquareMatrix | None
-        Matrix (NxN) of transition probabilities, $P_{ij}$. If `None`, it will
+    f : FloatVectorLike (N) | None
+        Vector of instantaneous monomer compositions, $f_i$.
+    r : FloatSquareMatrix (N, N) | None
+        Matrix of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
+    P : FloatSquareMatrix (N, N) | None
+        Matrix of transition probabilities, $P_{ij}$. If `None`, it will
         be computed internally. When calculating other quantities (e.g.,
         sequence lengths, tuples) that also depend on $P$, it is more efficient
         to precompute $P$ once and use it in all cases.
 
     Returns
     -------
-    FloatVector
-        Vector (N) of instantaneous copolymer compositions, $F_i$.
-
-    !!! note annotate "See also"
-
-        * [`inst_copolymer_binary`](inst_copolymer_binary.md):
-          specific method for binary systems.
-        * [`inst_copolymer_ternary`](inst_copolymer_ternary.md):
-          specific method for terpolymer systems.
-        * [`monomer_drift_multi`](monomer_drift_multi.md):
-          monomer composition drift.
-        * [`transitions_multi`](transitions_multi.md):
-          instantaneous transition probabilities.
+    FloatVector (N)
+        Vector of instantaneous copolymer compositions, $F_i$.
 
-    **References**
-
-    *   H. K. Frensdorff, R. Pariser; Copolymerization as a Markov Chain.
-        J. Chem. Phys. 1 November 1963; 39 (9): 2303-2309.
+    See also
+    --------
+    * [`inst_copolymer_binary`](inst_copolymer_binary.md):
+      specific method for binary systems.
+    * [`inst_copolymer_ternary`](inst_copolymer_ternary.md):
+      specific method for terpolymer systems.
+    * [`monomer_drift_multi`](monomer_drift_multi.md):
+      monomer composition drift.
+    * [`transitions_multi`](transitions_multi.md):
+      instantaneous transition probabilities.
 
     Examples
     --------
     >>> from polykin.copolymerization import inst_copolymer_multi
     >>> import numpy as np
 
     Define reactivity ratio matrix.
@@ -229,16 +229,16 @@
     b[-1] = 1.
     F = np.linalg.solve(A, b)
 
     return F
 
 
 def monomer_drift_multi(f0: FloatVectorLike,
-                        r: FloatSquareMatrix,
                         x: FloatVectorLike,
+                        r: FloatSquareMatrix,
                         rtol: float = 1e-4
                         ) -> FloatMatrix:
     r"""Compute the monomer composition drift for a multicomponent system.
 
     In a closed system, the drift in monomer composition is given by
     the solution of the following system of differential equations:
 
@@ -246,34 +246,36 @@
 
     with initial condition $f_i(0)=f_{i,0}$, where $f_i$ and $F_i$ are,
     respectively, the instantaneous comonomer and copolymer composition of
     monomer $i$, and $x$ is the total molar monomer conversion.
 
     Parameters
     ----------
-    f0 : FloatVectorLike
-        Vector (N) of initial instantaneous comonomer compositions.
-    r : FloatSquareMatrix
-        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
-    x : FloatVectorLike
-        Vector (M) of total monomer conversion values where the drift is to be
+    f0 : FloatVectorLike (N)
+        Vector of initial instantaneous comonomer compositions.
+    x : FloatVectorLike (M)
+        Vector of total monomer conversion values where the drift is to be
         evaluated.
+    r : FloatSquareMatrix (N, N)
+        Matrix of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
     rtol : float
-        Relative tolerance of ODE solver.
+        Relative tolerance of the ODE solver.
 
     Returns
     -------
-    FloatMatrix
-        Matrix (MxN) of monomer fraction of monomer $i$ at the specified
-        total monomer conversion(s), $f_i(x_j)$.
-
-    !!! note annotate "See also"
+    FloatMatrix (M, N)
+        Matrix of monomer fraction of monomer $i$ at the specified total
+        monomer conversions, $f_i(x_j)$.
 
-        * [`inst_copolymer_multi`](inst_copolymer_multi.md):
-          instantaneous copolymer composition.
+    See also
+    --------
+    * [`inst_copolymer_multi`](inst_copolymer_multi.md): 
+      instantaneous copolymer composition.
+    * [`monomer_drift_multi`](monomer_drift_multi.md):
+      specific method for binary systems.
 
     Examples
     --------
     >>> from polykin.copolymerization import monomer_drift_multi
     >>> import numpy as np
 
     Define reactivity ratio matrix.
@@ -284,15 +286,15 @@
     >>> r[2, 0] = 0.9
     >>> r[1, 2] = 0.4
     >>> r[2, 1] = 1.5
 
     Evaluate monomer drift.
     >>> f0 = [0.5, 0.3, 0.2]
     >>> x = [0.1, 0.5, 0.9, 0.99]
-    >>> f = monomer_drift_multi(f0, r, x)
+    >>> f = monomer_drift_multi(f0, x, r)
     >>> f
     array([[5.19230749e-01, 2.87888151e-01, 1.92881100e-01],
            [6.38387269e-01, 2.04571229e-01, 1.57041502e-01],
            [8.31725111e-01, 5.64177982e-03, 1.62633109e-01],
            [5.00285275e-01, 1.93845681e-07, 4.99714531e-01]])
 
     """
@@ -340,32 +342,32 @@
     **References**
 
     *   NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
         process modeling, Wiley, 1996, p. 178.
 
     Parameters
     ----------
-    f : FloatVectorLike
-        Vector (N) of instantaneous monomer compositions, $f_i$.
-    r : FloatSquareMatrix
-        Matrix (NxN) of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
+    f : FloatVectorLike (N)
+        Vector of instantaneous monomer compositions, $f_i$.
+    r : FloatSquareMatrix (N, N)
+        Matrix of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
 
     Returns
     -------
-    FloatSquareMatrix
-        Matrix (NxN) of transition probabilities, $P_{ij}$.
+    FloatSquareMatrix (N, N)
+        Matrix of transition probabilities, $P_{ij}$.
 
-    !!! note annotate "See also"
-
-        * [`inst_copolymer_multi`](inst_copolymer_multi.md):
-          instantaneous copolymer composition.
-        * [`sequence_multi`](sequence_multi.md):
-          instantaneous sequence lengths.
-        * [`tuples_multi`](tuples_multi.md):
-          instantaneous tuple fractions.
+    See also
+    --------
+    * [`inst_copolymer_multi`](inst_copolymer_multi.md):
+      instantaneous copolymer composition.
+    * [`sequence_multi`](sequence_multi.md):
+      instantaneous sequence lengths.
+    * [`tuples_multi`](tuples_multi.md):
+      instantaneous tuple fractions.
 
     Examples
     --------
     >>> from polykin.copolymerization import transitions_multi
     >>> import numpy as np
 
     Define reactivity ratio matrix.
@@ -419,33 +421,33 @@
     **References**
 
     * NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
     process modeling, Wiley, 1996, p. 177.
 
     Parameters
     ----------
-    Pself : FloatVectorLike
-        Vector (N) of self-transition probabilities, $P_{ii}$, corresponding to
+    Pself : FloatVectorLike (N)
+        Vector of self-transition probabilities, $P_{ii}$, corresponding to
         the diagonal of the matrix of transition probabilities.
-    k : int | IntArrayLike | None
+    k : int | IntArrayLike (M) | None
         Sequence length, i.e., number of consecutive units in a chain.
         If `None`, the number-average sequence length will be computed.
 
     Returns
     -------
-    FloatArray
+    FloatArray (N, M)
         If `k is None`, the number-average sequence lengths, $\bar{S}_i$.
         Otherwise, the sequence probabilities, $S_{i,k}$.
 
-    !!! note annotate "See also"
-
-        * [`transitions_multi`](transitions_multi.md):
-          instantaneous transition probabilities.
-        * [`tuples_multi`](tuples_multi.md):
-          instantaneous tuple fractions.
+    See also
+    --------
+    * [`transitions_multi`](transitions_multi.md):
+      instantaneous transition probabilities.
+    * [`tuples_multi`](tuples_multi.md):
+      instantaneous tuple fractions.
 
     Examples
     --------
     >>> from polykin.copolymerization import sequence_multi
     >>> from polykin.copolymerization import transitions_multi
     >>> import numpy as np
 
@@ -511,35 +513,35 @@
     **References**
 
     *   NA Dotson, R Galván, RL Laurence, and M Tirrel. Polymerization
         process modeling, Wiley, 1996, p. 179.
 
     Parameters
     ----------
-    P : FloatSquareMatrix
-        Matrix (NxN) of transition probabilities, $P_{ij}$.
+    P : FloatSquareMatrix (N, N)
+        Matrix of transition probabilities, $P_{ij}$.
     n : int
         Tuple length,.e.g monads (1), diads (2), triads (3), etc.
-    F : FloatVectorLike | None
-        Vector (N) of instantaneous copolymer composition, $F_i$. If `None`,
+    F : FloatVectorLike (N) | None
+        Vector of instantaneous copolymer composition, $F_i$. If `None`,
         the value will be computed internally. When calculating tuples of
         various lengths, it is more efficient to precompute $F$ and use it in
         all tuple cases.
 
     Returns
     -------
     dict[tuple[int, ...], float]
         Tuple of molar fractions.
 
-    !!! note annotate "See also"
-
-        * [`sequence_multi`](sequence_multi.md):
-          instantaneous sequence lengths.
-        * [`transitions_multi`](transitions_multi.md):
-          instantaneous transition probabilities.
+    See also
+    --------
+    * [`sequence_multi`](sequence_multi.md):
+      instantaneous sequence lengths.
+    * [`transitions_multi`](transitions_multi.md):
+      instantaneous transition probabilities.
 
     Examples
     --------
     >>> from polykin.copolymerization import tuples_multi
     >>> from polykin.copolymerization import transitions_multi
     >>> import numpy as np
 
@@ -609,16 +611,16 @@
     Parameters
     ----------
     Qe_values : list[tuple[float, float]]
         List (N) of Q-e values.
 
     Returns
     -------
-    FloatSquareMatrix
-        Reactivity ratio matrix (NxN).
+    FloatSquareMatrix (N, N)
+        Reactivity ratio matrix.
 
     Examples
     --------
     Estimate the reactivity ratio matrix for styrene (1), methyl
     methacrylate (2), and vinyl acetate(3) using Q-e values from the
     literature.
```

### Comparing `polykin-0.5.1/src/polykin/copolymerization/penultimate.py` & `polykin-0.5.2/src/polykin/copolymerization/penultimate.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/copolymerization/terminal.py` & `polykin-0.5.2/src/polykin/copolymerization/terminal.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,16 @@
         def df1dx(x_, f1_):
             F1_ = inst_copolymer_binary(f1_, *self.ri(f1_))
             return (f1_ - F1_)/(1. - x_ + eps)
 
         sol = solve_ivp(df1dx,
                         (0., max(x)),
                         f10,
-                        method='LSODA',
                         t_eval=x,
+                        method='LSODA',
                         vectorized=True,
                         rtol=1e-4)
         if sol.success:
             result = sol.y
             result = np.maximum(0., result)
             if result.shape[0] == 1:
                 result = result[0]
```

### Comparing `polykin-0.5.1/src/polykin/distributions/analyticaldistributions.py` & `polykin-0.5.2/src/polykin/distributions/analyticaldistributions.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/distributions/base.py` & `polykin-0.5.2/src/polykin/distributions/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/distributions/datadistribution.py` & `polykin-0.5.2/src/polykin/distributions/datadistribution.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/distributions/sampledata.py` & `polykin-0.5.2/src/polykin/distributions/sampledata.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/kinetics/arrhenius.py` & `polykin-0.5.2/src/polykin/kinetics/arrhenius.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     unit : str
         Unit of coefficient.
     symbol : str
         Symbol of coefficient $k$.
     name : str
         Name.
 
-    !!! note annotate "See also"
-
-        * [`Eyring`](Eyring.md): alternative method.
+    See also
+    --------
+    * [`Eyring`](Eyring.md): alternative method.
 
     """
 
     _pinfo = {'k0': ('#', True), 'EaR': ('K', True), 'T0': ('K', False)}
 
     def __init__(self,
                  k0: Union[float, FloatArrayLike],
```

### Comparing `polykin-0.5.1/src/polykin/kinetics/base.py` & `polykin-0.5.2/src/polykin/kinetics/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/kinetics/cldpropagation.py` & `polykin-0.5.2/src/polykin/kinetics/cldpropagation.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/kinetics/cldtermination.py` & `polykin-0.5.2/src/polykin/kinetics/cldtermination.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/kinetics/eyring.py` & `polykin-0.5.2/src/polykin/kinetics/eyring.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         Upper temperature bound.
         Unit = K.
     symbol : str
         Symbol of coefficient $k$.
     name : str
         Name.
 
-    !!! note annotate "See also"
-
-        * [`Arrhenius`](Arrhenius.md): alternative method.
+    See also
+    --------
+    * [`Arrhenius`](Arrhenius.md): alternative method.
 
     """
 
     _pinfo = {'DSa': ('J/(mol·K)', True),
               'DHa': ('J/mol', True), 'kappa': ('', False)}
 
     def __init__(self,
```

### Comparing `polykin-0.5.1/src/polykin/math/derivatives.py` & `polykin-0.5.2/src/polykin/math/derivatives.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/math/jcr.py` & `polykin-0.5.2/src/polykin/math/jcr.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,19 @@
         Color of ellipse contour and center.
     label : str | None
         Ellipse label.
     confint : bool
         If `True` the _individual_ confidence intervals of the parameters are
         represented as lines.
 
-    !!! note annotate "See also"
+    See also
+    --------
+    * [`confidence_region`](confidence_region.md): alternative method based on
+    rigorous approach for non-linear models.
 
-        * [`confidence_region`](confidence_region.md): alternative method
-        based on rigorous approach for non-linear models.
     """
 
     # Method implementation is specific for 2D
     npar = 2
     if len(center) != npar:
         raise ShapeError(f"`center` must be a vector of length {npar}.")
 
@@ -203,18 +204,18 @@
         insufficient.
 
     Returns
     -------
     tuple[FloatVector, FloatVector]
         Coordinates (x, y) of the confidence region.
 
-    !!! note annotate "See also"
-
-        * [`confidence_ellipse`](confidence_ellipse.md): alternative method
-        based on linear approximation.
+    See also
+    --------
+    * [`confidence_ellipse`](confidence_ellipse.md): alternative method based
+      on linear approximation.
 
     """
 
     # Method implementation is specific for 2D
     npar = 2
     if len(center) != npar:
         raise ShapeError(f"`center` must be a vector of length {npar}.")
```

### Comparing `polykin-0.5.1/src/polykin/properties/diffusion/liquid.py` & `polykin-0.5.2/src/polykin/properties/diffusion/liquid.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         unassociated: 1.0}.
 
     Returns
     -------
     float
         Diffusion coefficient of A in B at infinite dilution. Unit = m²/s.
 
-    !!! note annotate "See also"
-
-        * [`DL_Hayduk_Minhas`](DL_Hayduk_Minhas.md): alternative method.
+    See also
+    --------
+    * [`DL_Hayduk_Minhas`](DL_Hayduk_Minhas.md): alternative method.
 
     Examples
     --------
     Estimate the diffusion coefficient of vinyl chloride through liquid water.
 
     >>> from polykin.properties.diffusion import DL_Wilke_Chang
     >>> D = DL_Wilke_Chang(
@@ -112,17 +112,17 @@
         Viscostity of solvent B. Unit = Pa.s.
 
     Returns
     -------
     float
         Diffusion coefficient of A in B at infinite dilution. Unit = m²/s.
 
-    !!! note annotate "See also"
-
-        * [`DL_Wilke_Chang`](DL_Wilke_Chang.md): alternative method.
+    See also
+    --------
+    * [`DL_Wilke_Chang`](DL_Wilke_Chang.md): alternative method.
 
     Examples
     --------
     Estimate the diffusion coefficient of vinyl chloride through liquid water.
 
     >>> from polykin.properties.diffusion import DL_Hayduk_Minhas
     >>> D = DL_Hayduk_Minhas(
```

### Comparing `polykin-0.5.1/src/polykin/properties/diffusion/vapor.py` & `polykin-0.5.2/src/polykin/properties/diffusion/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/diffusion/vrentasduda.py` & `polykin-0.5.2/src/polykin/properties/diffusion/vrentasduda.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/equations/base.py` & `polykin-0.5.2/src/polykin/properties/equations/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/equations/dippr.py` & `polykin-0.5.2/src/polykin/properties/equations/dippr.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/equations/vapor_pressure.py` & `polykin-0.5.2/src/polykin/properties/equations/vapor_pressure.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,21 @@
     unit : str
         Unit of vapor pressure.
     symbol : str
         Symbol of vapor pressure.
     name : str
         Name.
 
-    !!! note annotate "See also"
+    See also
+    --------
+    * [`DIPPR101`](./#polykin.properties.equations.dippr.DIPPR101):
+      alternative method, applicable to wider temperature ranges.
+    * [`Wagner`](./#polykin.properties.equations.vapor_pressure.Wagner):
+      alternative method, applicable to wider temperature ranges.
 
-        * [`DIPPR101`](./#polykin.properties.equations.dippr.DIPPR101):
-        alternative method, applicable to wider temperature ranges.
-        * [`Wagner`](./#polykin.properties.equations.vapor_pressure.Wagner):
-        alternative method, applicable to wider temperature ranges.
     """
 
     _pinfo = {'A': ('', True), 'B': ('K', True), 'C': ('K', True),
               'base10': ('', False)}
 
     def __init__(self,
                  A: float,
```

### Comparing `polykin-0.5.1/src/polykin/properties/equations/viscosity.py` & `polykin-0.5.2/src/polykin/properties/equations/viscosity.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/mixing_rules.py` & `polykin-0.5.2/src/polykin/properties/mixing_rules.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/Flory_parameters.tsv` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/Flory_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/Tait_parameters.tsv` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/Tait_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/base.py` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/eos.py` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/eos.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/pvt_polymer/tait.py` & `polykin-0.5.2/src/polykin/properties/pvt_polymer/tait.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/thermal_conductivity/liquid.py` & `polykin-0.5.2/src/polykin/properties/thermal_conductivity/liquid.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/thermal_conductivity/vapor.py` & `polykin-0.5.2/src/polykin/properties/thermal_conductivity/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/vaporization_enthalpy.py` & `polykin-0.5.2/src/polykin/properties/vaporization_enthalpy.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/viscosity/liquid.py` & `polykin-0.5.2/src/polykin/properties/viscosity/liquid.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/properties/viscosity/vapor.py` & `polykin-0.5.2/src/polykin/properties/viscosity/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/stepgrowth/solutions.py` & `polykin-0.5.2/src/polykin/stepgrowth/solutions.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/base.py` & `polykin-0.5.2/src/polykin/thermo/acm/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/floryhuggins.py` & `polykin-0.5.2/src/polykin/thermo/acm/floryhuggins.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,18 +299,19 @@
         (but not checked) that $\chi_{ij}=\chi_{ji}$ and $\chi_{ii}=0$.
 
     Returns
     -------
     FloatVector
         Activities of all components.
 
-    !!! note annotate "See also"
+    See also
+    --------
+    * [`FloryHuggins2_activity`](FloryHuggins2_activity.md): equivalent
+      method for binary solvent-polymer systems.
 
-        * [`FloryHuggins2_activity`](FloryHuggins2_activity.md): equivalent
-        method for binary solvent-polymer systems.
     """
     A = dot(phi, 1/m)
     B = dot(chi, phi)
     C = 0.5*dot(phi, dot(phi, chi))
     return phi*exp(1 - m*(A - B + C))
 
 
@@ -357,18 +358,18 @@
         Solvent-polymer interaction parameter, $\chi$.
 
     Returns
     -------
     FloatVector
         Activity of the solvent.
 
-    !!! note annotate "See also"
-
-        * [`FloryHuggins_activity`](FloryHuggins_activity.md): equivalent
-        method for multicomponent systems.
+    See also
+    --------
+    * [`FloryHuggins_activity`](FloryHuggins_activity.md): equivalent method
+      for multicomponent systems.
 
     Examples
     --------
     Calculate the activity of ethylbenzene in a ethylbenzene-polybutadiene
     solution with 25 wt% solvent content. Assume $\chi=0.29$.
     >>> from polykin.thermo.acm import FloryHuggins2_gamma
     >>> gamma = FloryHuggins2_gamma(phi1=0.25, m=1e6, chi=0.29)
```

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/ideal.py` & `polykin-0.5.2/src/polykin/thermo/acm/ideal.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/nrtl.py` & `polykin-0.5.2/src/polykin/thermo/acm/nrtl.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     e : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     f : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     name: str
         Name.
 
-    !!! note annotate "See also"
-
-        * [`NRTL_gamma`](NRTL_gamma.md): related activity coefficient method.
+    See also
+    --------
+    * [`NRTL_gamma`](NRTL_gamma.md): related activity coefficient method.
 
     """
 
     _a: FloatSquareMatrix
     _b: FloatSquareMatrix
     _c: FloatSquareMatrix
     _d: FloatSquareMatrix
@@ -227,17 +227,18 @@
         checked) that $\alpha_{ij}=\alpha_{ji}$.
 
     Returns
     -------
     FloatVector (N)
         Activity coefficients of all components.
 
-    !!! note annotate "See also"
+    See also
+    --------
+    * [`NRTL`](NRTL.md): related class.
 
-        * [`NRTL`](NRTL.md): related class.
     """
 
     G = exp(-alpha*tau)
 
     # N = x.size
     # A = np.empty(N)
     # B = np.empty(N)
```

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/polynrtl.py` & `polykin-0.5.2/src/polykin/thermo/acm/polynrtl.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/uniquac.py` & `polykin-0.5.2/src/polykin/thermo/acm/uniquac.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,17 @@
     c : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     d : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     name : str
         Name.
 
-    !!! note annotate "See also"
-
-        * [`UNIQUAC_gamma`](UNIQUAC_gamma.md): related activity coefficient
-          method.
+    See also
+    --------
+    * [`UNIQUAC_gamma`](UNIQUAC_gamma.md): related activity coefficient method.
 
     """
 
     _q: FloatVector
     _r: FloatVector
     _a: FloatSquareMatrix
     _b: FloatSquareMatrix
@@ -232,17 +231,17 @@
         that $\tau_{ii}=1$.
 
     Returns
     -------
     FloatVector (N)
         Activity coefficients of all components.
 
-    !!! note annotate "See also"
-
-        * [`UNIQUAC`](UNIQUAC.md): related class.
+    See also
+    --------
+    * [`UNIQUAC`](UNIQUAC.md): related class.
 
     """
 
     J = r/dot(x, r)
     L = q/dot(x, q)
     theta = x*L
     s = dot(theta, tau)
```

### Comparing `polykin-0.5.1/src/polykin/thermo/acm/wilson.py` & `polykin-0.5.2/src/polykin/thermo/acm/wilson.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     c : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     d : FloatSquareMatrix (N,N) | None
         Matrix of interaction parameters, by default 0.
     name: str
         Name.
 
-    !!! note annotate "See also"
-
-        * [`Wilson_gamma`](Wilson_gamma.md): related activity coefficient
-        method.
+    See also
+    --------
+    * [`Wilson_gamma`](Wilson_gamma.md): related activity coefficient
+    method.
 
     """
 
     _a: FloatSquareMatrix
     _b: FloatSquareMatrix
     _c: FloatSquareMatrix
     _d: FloatSquareMatrix
@@ -162,13 +162,14 @@
         checked) that $\Lambda_{ii}=1$.
 
     Returns
     -------
     FloatVector (N)
         Activity coefficients of all components.
 
-    !!! note annotate "See also"
+    See also
+    --------
+    * [`Wilson`](Wilson.md): related class.
 
-        * [`Wilson`](Wilson.md): related class.
     """
     A = dot(Lambda, x)
     return exp(1. - dot(x/A, Lambda))/A
```

### Comparing `polykin-0.5.1/src/polykin/thermo/eos/base.py` & `polykin-0.5.2/src/polykin/thermo/eos/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/eos/cubic.py` & `polykin-0.5.2/src/polykin/thermo/eos/cubic.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/eos/idealgas.py` & `polykin-0.5.2/src/polykin/thermo/eos/idealgas.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/thermo/eos/virial.py` & `polykin-0.5.2/src/polykin/thermo/eos/virial.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/utils/math.py` & `polykin-0.5.2/src/polykin/utils/math.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/utils/tools.py` & `polykin-0.5.2/src/polykin/utils/tools.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/src/polykin/utils/types.py` & `polykin-0.5.2/src/polykin/utils/types.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.1/PKG-INFO` & `polykin-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polykin
-Version: 0.5.1
+Version: 0.5.2
 Summary: A polymerization kinetics library.
 Home-page: https://hugomvale.github.io/polykin/
 License: MIT
 Keywords: polymer,polymerization,kinetics,reaction
 Author: HugoMVale
 Author-email: 57530119+HugoMVale@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -45,15 +45,15 @@
   - [x] UNIQUAC
   - [x] Wilson
 - Copolymerization
   - [x] Implicit penultimate model
   - [x] Penultimate model
   - [x] Terminal model
   - [x] Mayo-Lewis equation (binary, ternary and multicomponent)
-  - [x] Monomer dift equation (multicomponent)
+  - [x] Monomer drift equation (binary and multicomponent)
   - [ ] Fitting methods
 - Equations of state
   - [50%] Cubic (Redlich-Kwong, Soave, Peng-Robinson)
   - [x] Ideal gas
   - [ ] Sanchez-Lacombe
   - [x] Virial equation
 - [ ] Database
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polykin Version: 0.5.1 Summary: A polymerization
+Metadata-Version: 2.1 Name: polykin Version: 0.5.2 Summary: A polymerization
 kinetics library. Home-page: https://hugomvale.github.io/polykin/ License: MIT
 Keywords: polymer,polymerization,kinetics,reaction Author: HugoMVale Author-
 email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
@@ -21,31 +21,32 @@
 github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-
 commit/HugoMVale/polykin) PolyKin is an open-source polymerization kinetics
 library for Python. It is still at an early development stage, but the
 following modules can already be used: - Activity coefficient models - [x]
 Ideal solution - [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL - [x] UNIQUAC -
 [x] Wilson - Copolymerization - [x] Implicit penultimate model - [x]
 Penultimate model - [x] Terminal model - [x] Mayo-Lewis equation (binary,
-ternary and multicomponent) - [x] Monomer dift equation (multicomponent) - [ ]
-Fitting methods - Equations of state - [50%] Cubic (Redlich-Kwong, Soave, Peng-
-Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe - [x] Virial equation - [ ]
-Database - Distributions - [x] Flory - [ ] Gold - [x] Log-normal - [x] Poison -
-[x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x] Eyring - [x] Propagation half-
-length - [x] Termination composite model - Math - [x] Joint confidence regions
-- [ ] Models - Physical property correlations - [x] Antoine - [x] DIPPR - [x]
-Wagner - [x] Yaws - Step-growth polymerization - [x] Analytical solutions for
-$M_n$ and $M_w$ - Transport properties (estimation methods, mixing rules, etc.)
-- Diffusivity - [x] Binary gas mixtures - [x] Binary liquid mixtures - [x]
-Binary polymer solutions - [ ] Multicomponent polymer solutions - Thermal
-conductivity - [x] Gases - [x] Liquids - [ ] Polymer solutions - Viscosity -
-[x] Gases - [x] Liquids - [ ] Polymer solutions ## Documentation Please refer
-to the package [homepage](https://hugomvale.github.io/polykin/). ## Tutorials
-The main features of PolyKin are explained and illustrated through a series of
-[tutorials](https://hugomvale.github.io/polykin/tutorials/) based on Jupyter
-[notebooks](https://github.com/HugoMVale/polykin/tree/main/docs/tutorials),
-which can be launched online via Binder.
+ternary and multicomponent) - [x] Monomer drift equation (binary and
+multicomponent) - [ ] Fitting methods - Equations of state - [50%] Cubic
+(Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe -
+[x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ] Gold - [x]
+Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x]
+Eyring - [x] Propagation half-length - [x] Termination composite model - Math -
+[x] Joint confidence regions - [ ] Models - Physical property correlations -
+[x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth polymerization -
+[x] Analytical solutions for $M_n$ and $M_w$ - Transport properties (estimation
+methods, mixing rules, etc.) - Diffusivity - [x] Binary gas mixtures - [x]
+Binary liquid mixtures - [x] Binary polymer solutions - [ ] Multicomponent
+polymer solutions - Thermal conductivity - [x] Gases - [x] Liquids - [ ]
+Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ] Polymer solutions
+## Documentation Please refer to the package [homepage](https://
+hugomvale.github.io/polykin/). ## Tutorials The main features of PolyKin are
+explained and illustrated through a series of [tutorials](https://
+hugomvale.github.io/polykin/tutorials/) based on Jupyter [notebooks](https://
+github.com/HugoMVale/polykin/tree/main/docs/tutorials), which can be launched
+online via Binder.
                            _[_M_W_D_ _o_f_ _a_ _p_o_l_y_m_e_r_ _b_l_e_n_d_]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
 repository: ```console git clone https://github.com/HugoMVale/polykin.git cd
 polykin pip install . # poetry install ```
```

