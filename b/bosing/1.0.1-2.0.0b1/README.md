# Comparing `tmp/bosing-1.0.1.tar.gz` & `tmp/bosing-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data
```

## Comparing `bosing-1.0.1.tar` & `bosing-2.0.0b1.tar`

### file list

```diff
@@ -1,131 +1,42 @@
--rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.1/.editorconfig
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.1/.gitattributes
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 bosing-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.1/Bosing.sln
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.1/Directory.Build.props
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bosing-1.0.1/VERSION.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.1/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.1/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.1/exclusion.dic
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 bosing-1.0.1/ruff_defaults.toml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 bosing-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/Program.cs
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.1/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/__init__.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/_native.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/_utils.py
--rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 bosing-1.0.1/python/bosing/models.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/Makefile
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/api.rst
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/conf.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/index.rst
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/instruction.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/make.bat
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/quickstart.rst
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/requirements.txt
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/schedule.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.1/python/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.1/python/example/schedule.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.1/python/example/schedule_stress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bosing-1.0.1/python/tests/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bosing-1.0.1/python/tests/test_basic.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadChain.cs
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadCoefficients.cs
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BiquadFilter.cs
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Bosing.csproj
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/BosingOptions.cs
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ComplexReadOnlySpan.cs
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ComplexSpan.cs
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Envelope.cs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeCacheKey.cs
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeInfo.cs
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/EnvelopeSample.cs
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/FirCoefficients.cs
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/HannPulseShape.cs
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/IPulseShape.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/InterpolatedPulseShape.cs
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/IqPair.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/MathUtils.cs
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PhaseTrackingTransform.cs
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PooledComplexArray.cs
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PostProcessTransform.cs
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/PulseList.cs
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/SignalFilter.cs
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/TimeAxisUtils.cs
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/TrianglePulseShape.cs
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/ValueArray.cs
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/WaveformSampler.cs
--rw-r--r--   0        0        0    30212 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/WaveformUtils.cs
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/AbsoluteSchedule.cs
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Alignment.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ArrangeOption.cs
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/BarrierElement.cs
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridLength.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridLengthUnit.cs
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/GridSchedule.cs
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/PlayElement.cs
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/RepeatElement.cs
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Schedule.cs
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ScheduleElement.cs
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SetFrequencyElement.cs
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SetPhaseElement.cs
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ShiftFrequencyElement.cs
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/ShiftPhaseElement.cs
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/StackSchedule.cs
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/SwapPhaseElement.cs
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing/Schedules/Thickness.cs
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Api.cs
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Bosing.Aot.csproj
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/ScheduleRunner.cs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/UnsafeMemoryManager.cs
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/BarrierElementDto.cs
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/BiquadDto.cs
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ChannelInfo.cs
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/GridScheduleDto.cs
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/HannShapeInfo.cs
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/IqCalibration.cs
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/OptionsDto.cs
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/PlayElementDto.cs
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/RepeatElementDto.cs
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ScheduleElementDto.cs
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ScheduleRequest.cs
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SetPhaseElementDto.cs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShapeInfo.cs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/StackScheduleDto.cs
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.1/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Bosing.Tests.csproj
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/EnvelopeInfoTests.cs
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/HannPulseShapeTests.cs
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/IntegrationTests.cs
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/IqPairTests.cs
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/MathUtilsTests.cs
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/PooledComplexArrayTests.cs
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/PulseListTests.cs
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/TimeAxisUtilsTests.cs
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/ToleranceComparer.cs
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/TrianglePulseShapeTests.cs
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Usings.cs
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/WaveformUtilsTests.cs
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/ScheduleTests.cs
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.1/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bosing-1.0.1/README.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 bosing-1.0.1/hatch_build.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bosing-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bosing-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 bosing-2.0.0b1/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6307 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-20 18:18:31.000000 bosing-2.0.0b1/LICENSE.txt
+-rw-r--r--   0     1001      127     1348 2024-04-20 18:18:31.000000 bosing-2.0.0b1/README.md
+-rw-r--r--   0     1001      127    10174 2024-04-20 18:18:31.000000 bosing-2.0.0b1/bosing.pyi
+-rw-r--r--   0     1001      127      634 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/conf.py
+-rw-r--r--   0     1001      127     1262 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/index.rst
+-rw-r--r--   0     1001      127     2259 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/quickstart.rst
+-rw-r--r--   0     1001      127       16 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/schedule.rst
+-rw-r--r--   0     1001      127     1138 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/flexible.py
+-rw-r--r--   0     1001      127      521 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/hann.py
+-rw-r--r--   0     1001      127      770 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/interp.py
+-rw-r--r--   0     1001      127      682 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/overlap.py
+-rw-r--r--   0     1001      127     2219 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/schedule.py
+-rw-r--r--   0     1001      127     1879 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-20 18:18:31.000000 bosing-2.0.0b1/ruff_defaults.toml
+-rw-r--r--   0     1001      127    48283 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/lib.rs
+-rw-r--r--   0     1001      127     9860 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/sampler.rs
+-rw-r--r--   0     1001      127     2479 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7387 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3311 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2349 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3944 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5741 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11082 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule.rs
+-rw-r--r--   0     1001      127     4160 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-20 18:18:31.000000 bosing-2.0.0b1/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-20 18:18:31.000000 bosing-2.0.0b1/tests/__init__.py
+-rw-r--r--   0     1001      127     1171 2024-04-20 18:18:31.000000 bosing-2.0.0b1/tests/test_basic.py
+-rw-r--r--   0     1001      127    13735 2024-04-20 18:18:40.000000 bosing-2.0.0b1/Cargo.lock
+-rw-r--r--   0     1001      127     1879 2024-04-20 18:18:31.000000 bosing-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bosing-1.0.1/.readthedocs.yaml` & `bosing-2.0.0b1/.readthedocs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 version: 2
 
 # Set the OS, Python version and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
     python: "3.12"
-    # You can also specify other tool versions:
-    # nodejs: "20"
-    # rust: "1.70"
-    # golang: "1.20"
-  apt_packages:
-    - dotnet-sdk-8.0
+    rust: "1.75"
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
-  configuration: python/docs/conf.py
+  configuration: docs/conf.py
   # You can configure Sphinx to use a different builder, for instance use the dirhtml builder for simpler URLs
   # builder: "dirhtml"
   # Fail on all warnings to avoid broken references
   # fail_on_warning: true
 
 # Optionally build your docs in additional formats such as PDF and ePub
 # formats:
@@ -30,10 +25,10 @@
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
-    - requirements: python/docs/requirements.txt
+    - requirements: docs/requirements.txt
     - method: pip
-      path: .
+      path: .
```

### Comparing `bosing-1.0.1/ruff_defaults.toml` & `bosing-2.0.0b1/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.1/python/docs/Makefile` & `bosing-2.0.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-1.0.1/python/docs/conf.py` & `bosing-2.0.0b1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.viewcode",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
+    "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "matplotlib.sphinxext.plot_directive",
 ]
 
-autodoc_typehints = "description"
 autosummary_imported_members = True
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/", None),
+    "matplotlib": ("https://matplotlib.org/stable", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
 }
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
```

### Comparing `bosing-1.0.1/python/docs/index.rst` & `bosing-2.0.0b1/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 
 ``bosing`` 是一个用于生成微波波形的 Python 库, 通过类似 HTML DOM 的结构编排波形,
 既可直接用于生成简单的波形序列, 也可作为 `qiskit <https://qiskit.org>`_ 等量子门
 线路优化器的后端, 生成复杂的微波波形. 目前实现的功能有:
 
 * 脉冲编排: 通过 :class:`Stack` 等控制波形时序
 * 自定义波形: 通过 :class:`Interp` 自定义插值波形
-* 滤波器: 通过 :attr:`Channel.iir` 和 :attr:`Channel.fir` 添加滤波器
 
 安装
 ----
 
 .. code-block:: console
-   
+
     $ pip install bosing
 
 
 从源码安装
 ----------
 
-#. 安装 `.NET 8.0 SDK <https://dotnet.microsoft.com/en-us/download>`_
+#. 安装 Rust toolchain 1.74+
 #. 安装 Python 3.8+
 #. Clone 本项目并安装
 
     .. code-block:: console
 
         $ git clone https://github.com/kahojyun/Bosing.git
         $ cd Bosing
```

### Comparing `bosing-1.0.1/python/docs/instruction.rst` & `bosing-2.0.0b1/docs/instruction.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 波形指令
 ========
 
-.. currentmodule:: bosing.models
+.. currentmodule:: bosing
 
 ``bosing`` 通过一系列的指令控制波形的生成, 目前支持的指令有:
 
 :class:`Play`
     在指定通道上添加波形
 
 :class:`ShiftPhase`
@@ -78,11 +78,11 @@
     \phi_c^{(1)'}(\tau) = \phi_c^{(2)}(\tau) \\
     \phi_c^{(2)'}(\tau) = \phi_c^{(1)}(\tau)
 
 最后生成波形时, ``bosing`` 采用的 I, Q 通道混频公式为:
 
 .. math::
 
-    I(t) = E(t)\cos(\phi_p(t)) \\
-    Q(t) = E(t)\sin(\phi_p(t))
+    I(t) = E(t)\cos(2\pi\phi_p(t)) \\
+    Q(t) = E(t)\sin(2\pi\phi_p(t))
 
 其中 :math:`E(t)` 为包络.
```

### Comparing `bosing-1.0.1/python/docs/make.bat` & `bosing-2.0.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-1.0.1/python/docs/schedule.rst` & `bosing-2.0.0b1/docs/schedule.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 波形编排
 ========
 
-.. currentmodule:: bosing.models
+.. currentmodule:: bosing
 
 ``bosing`` 使用类似 HTML, XAML 的结构来描述波形序列, 用户可以定义基础的波形,
 然后通过组合的方式来构建复杂的波形序列. 基础元素有 :doc:`instruction`:
 
 * :class:`Play`
 * :class:`ShiftPhase`
 * :class:`SetPhase`
@@ -41,16 +41,16 @@
 --------
 
 每个元素都有以下基础属性:
 
 :attr:`Element.margin`
     元素前后额外占用的时间, 默认为 ``0``.
 
-:attr:`Element.visibility`
-    元素是否生效, 如果为 ``False`` 虽然会占用布局空间, 但是不会执行相应指令.
+:attr:`Element.phantom`
+    元素是否生效, 如果为 ``True`` 虽然会占用布局空间, 但是不会执行相应指令.
 
 :attr:`Element.alignment`
     元素在容器中的对齐方式, 目前只有 :class:`Grid` 会使用该属性, 其他布局会忽略
     该属性.
 
 :attr:`Element.duration`
     元素的持续时间, 默认为 ``None``, 由布局系统根据子元素计算.
@@ -68,26 +68,26 @@
     ``0.3`` 而不是 ``0.2``.
 
 .. note::
 
     GUI 布局中如果子元素的大小超过了容器的大小, 布局系统会裁剪子元素. 但是在波形
     计算中, 往往需要保留子元素的完整波形, 因此一旦出现超出容器的情况会抛出异常.
 
-.. note:: 
+.. note::
 
     当 :attr:`Element.duration`, :attr:`Element.max_duration`,
     :attr:`Element.min_duration` 三个属性同时存在且存在冲突时, 优先级为
     ``min_duration > max_duration > duration``.
 
 
 Stack 布局
 ----------
 
 在保持子元素前后顺序不变的前提下, 按照 :attr:`Stack.direction` 指定的方向排列子
-元素, 默认为 :attr:`ArrangeDirection.BACKWARDS`, 子元素尽量靠后排列. 如果需要同
+元素, 默认为 :attr:`Direction.Backward`, 子元素尽量靠后排列. 如果需要同
 步多个通道, 可以使用 :class:`Barrier`. 子元素的 :attr:`Element.alignment` 属性会
 被忽略, 持续时间尽可能短.
 
 
 Absolute 布局
 -------------
 
@@ -95,15 +95,15 @@
 忽略, 持续时间尽可能短. 子元素的位置非负, 容器的持续时间记录为起点到最晚结束的子
 元素的终点.
 
 添加子元素时需要指定位置, 默认为 ``0``.
 
 .. code-block:: python
 
-    absolute = Absolute().with_children(
+    absolute = Absolute(
         Play(...),
         (1e-9, Play(...)),
         (2e-9, Stack(...)),
     )
 
 
 Grid 布局
@@ -118,27 +118,27 @@
 添加子元素时需要指定列, 默认为 ``0``, 以及跨列数, 默认为 ``1``, 如果超出了容器的
 列数会当作最后一列处理.
 
 .. code-block:: python
 
     grid = Grid(columns=["*", "*", "*"]).with_children(
         Play(...),
-        (1, Play(...)),
-        (0, 3, Stack(...)),
+        (Play(...), 1),
+        (Stack(...), 0, 3),
     )
 
 .. tip::
 
     指定 column 宽度时, 可以使用 ``"Auto"``, ``"*"``, ``"2*"`` 等形式.
 
     .. code-block:: python
 
         grid = Grid(columns=["Auto", "*", "2*", 30e-9])
 
-.. caution:: 
+.. caution::
 
     当可用时长较小时, 无法保证按比例分配 ``Star`` 长度的列.
 
 
 布局算法
 --------
 
@@ -151,15 +151,15 @@
 
 使用时可以给最顶层的容器指定 :attr:`Element.duration`, 限制布局的持续时间.
 
 
 执行顺序
 --------
 
-.. caution:: 
+.. caution::
 
     在布局完成后, 会按照子元素插入顺序遍历执行, 与布局得到的元素位置无关.
 
 
 波形对齐
 --------
```

### Comparing `bosing-1.0.1/python/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.1/python/example/schedule.py` & `bosing-2.0.0b1/example/schedule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,70 @@
-"""An example of using bosing to generate a pulse sequence.
-"""
-
-import math
-from time import perf_counter
+"""An example of using bosing to generate a pulse sequence."""
 
 import numpy as np
 from matplotlib import pyplot as plt
-from scipy import signal
-
-from bosing import *
-
-
-def get_biquad(amp, tau, fs):
-    z = -1 / (tau * (1 + amp))
-    p = -1 / tau
-    k = 1 + amp
-    z, p, k = signal.bilinear_zpk([z], [p], k, fs)
-    sos = signal.zpk2sos(p, z, 1 / k)
-    return Biquad(sos[0][0], sos[0][1], sos[0][2], sos[0][4], sos[0][5])
-
-
-def get_iq_calibration(ratio, phase, offset_i, offset_q):
-    return IqCali(1, -math.tan(phase), 0, ratio / math.cos(phase), offset_i, offset_q)
+from scipy.interpolate import make_interp_spline
 
+from bosing import Absolute, Barrier, Channel, Grid, Hann, Interp, Play, Repeat, ShiftPhase, Stack, generate_waveforms
 
 if __name__ == "__main__":
-    t0 = perf_counter()
-
-    bq = get_biquad(-0.1, 20e-9, 2e9)
-    fir = signal.firwin(5, 100e6, fs=2e9)
+    length = 100000
     channels = [
-        Channel(
-            "xy0",
-            0,
-            2e9,
-            100000,
-            iq_calibration=get_iq_calibration(1.1, math.pi / 3, 0, 0),
-        ),
-        Channel("xy1", 0, 2e9, 100000),
-        Channel("u0", 0, 2e9, 100000, iir=[bq]),
-        Channel("u1", 0, 2e9, 100000, iir=[bq], fir=fir),
-        Channel("m0", 0, 2e9, 100000),
+        Channel("xy0", 0, 2e9, length),
+        Channel("xy1", 0, 2e9, length),
+        Channel("u0", 0, 2e9, length),
+        Channel("u1", 0, 2e9, length),
+        Channel("m0", 0, 2e9, length),
     ]
     c = {ch.name: i for i, ch in enumerate(channels)}
     halfcos = np.sin(np.linspace(0, np.pi, 10))
+    interp = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
     shapes = [
         Hann(),
-        Interp(np.linspace(-0.5, 0.5, 10), halfcos),
+        Interp(interp.t, interp.c, interp.k),
     ]
-    s = {"hann": 0, "rect": -1, "halfcos": 1}
+    s = {"hann": 0, "rect": None, "halfcos": 1}
 
-    measure = Absolute().with_children(
-        Play(c["m0"], 0.1, s["hann"], 30e-9, plateau=1e-6, frequency=123e6),
-        Play(c["m0"], 0.15, s["hann"], 30e-9, plateau=1e-6, frequency=-233e6),
+    measure = Absolute(
+        Play(c["m0"], s["hann"], 0.1, 30e-9, plateau=1e-6, frequency=123e6),
+        Play(c["m0"], s["hann"], 0.15, 30e-9, plateau=1e-6, frequency=-233e6),
     )
-    c01 = Stack().with_children(
-        Play(c["u0"], 0.5, s["rect"], 50e-9),
-        Play(c["u1"], 0.5, s["rect"], 50e-9),
+    c01 = Stack(
+        Play(c["u0"], s["rect"], 0.5, 50e-9),
+        Play(c["u1"], s["rect"], 0.5, 50e-9),
         ShiftPhase(c["xy0"], 0.1),
         ShiftPhase(c["xy1"], 0.2),
     )
-    x0 = Play(c["xy0"], 0.3, s["hann"], 50e-9, drag_coef=5e-10)
-    x1 = Play(c["xy1"], 0.4, s["hann"], 100e-9, drag_coef=3e-10)
-    x_group = Grid().with_children(
-        Stack([x0], alignment="center"),
-        Stack([x1], alignment="center"),
+    x0 = Play(c["xy0"], s["hann"], 0.3, 50e-9, drag_coef=5e-10)
+    x1 = Play(c["xy1"], s["hann"], 0.4, 100e-9, drag_coef=3e-10)
+    x_group = Grid(
+        Stack(x0, alignment="center"),
+        Stack(x1, alignment="center"),
     )
 
-    schedule = Stack(duration=49.9e-6).with_children(
+    schedule = Stack(duration=50e-6).with_children(
         Repeat(
-            Stack().with_children(
+            Stack(
                 x_group,
                 Barrier(duration=15e-9),
                 c01,
             ),
             count=200,
             spacing=15e-9,
         ),
         Barrier(duration=15e-9),
         measure,
+        Barrier(duration=15e-9),
     )
 
-    options = Options(time_tolerance=1e-13)
-
-    t1 = perf_counter()
-
-    result = generate_waveforms(channels, shapes, schedule, options=options)
-
-    t2 = perf_counter()
+    result = generate_waveforms(channels, shapes, schedule, time_tolerance=1e-13)
 
-    print(f"Build time: {t1 - t0:.3f}s")
-    print(f"Run time: {t2 - t1:.3f}s")
-
-    t = np.arange(100000) / 2e9
-    plt.plot(t, result["xy0"][0])
-    plt.plot(t, result["xy0"][1])
-    plt.plot(t, result["xy1"][0])
-    plt.plot(t, result["xy1"][1])
-    plt.plot(t, signal.lfilter(fir, [1], result["u0"][0]))
-    plt.plot(t, signal.lfilter(fir, [1], result["u0"][1]))
-    plt.plot(t, result["u1"][0])
-    plt.plot(t, result["u1"][1])
-    plt.plot(t, result["m0"][0])
-    plt.plot(t, result["m0"][1])
+    t = np.arange(length) / 2e9
+    plt.plot(t, result["xy0"].real)
+    plt.plot(t, result["xy0"].imag)
+    plt.plot(t, result["xy1"].real)
+    plt.plot(t, result["xy1"].imag)
+    plt.plot(t, result["u1"].real)
+    plt.plot(t, result["u1"].imag)
+    plt.plot(t, result["m0"].real)
+    plt.plot(t, result["m0"].imag)
     plt.show()
```

### Comparing `bosing-1.0.1/python/tests/test_basic.py` & `bosing-2.0.0b1/tests/test_basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 
 import bosing
 
 
 def test_basic():
     channels = [bosing.Channel("xy0", 100e6, 2e9, 100000)]
     shapes = [bosing.Hann()]
-    schedule = bosing.Stack(duration=49.9e-6).with_children(
-        bosing.Play(0, 0.1, 0, 100e-9)
-    )
+    schedule = bosing.Stack(duration=49.9e-6).with_children(bosing.Play(0, 0, 0.1, 100e-9))
     result = bosing.generate_waveforms(channels, shapes, schedule)
     assert "xy0" in result
-    i, q = result["xy0"]
-    assert len(i) == len(q)
-    assert len(i) == 100000
-    assert i[0] == 0
-    assert i[-1] == 0
-    assert np.any(i != 0)
-    assert q[0] == 0
-    assert q[-1] == 0
-    assert np.any(q != 0)
+    w = result["xy0"]
+    assert len(w) == 100000
+    assert w[0] == 0
+    assert w[-1] == 0
+    assert np.any(w != 0)
 
 
 def test_mixing():
     shapes = [bosing.Hann()]
     schedule = bosing.Stack(duration=500e-9).with_children(
         bosing.Play(
             channel_id=0,
@@ -34,17 +28,15 @@
         ),
         bosing.Barrier(duration=10e-9),
     )
     freq = 30e6
 
     channels = [bosing.Channel("xy", freq, 2e9, 1000)]
     result = bosing.generate_waveforms(channels, shapes, schedule)
-    i1, q1 = result["xy"]
-    w1 = i1 + 1j * q1
+    w1 = result["xy"]
 
     channels = [bosing.Channel("xy", 0, 2e9, 1000)]
     result = bosing.generate_waveforms(channels, shapes, schedule)
-    i2, q2 = result["xy"]
-    w2 = i2 + 1j * q2
+    w2 = result["xy"]
     w2 = w2 * np.exp(1j * (2 * np.pi * freq * np.arange(1000) / 2e9))
 
     assert np.allclose(w1, w2)
```

### Comparing `bosing-1.0.1/LICENSE.txt` & `bosing-2.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-1.0.1/README.md` & `bosing-2.0.0b1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,53 @@
 pip install bosing
 ```
 
 ## Documentation
 
 Docs are hosted on [Read the Docs](http://bosing.readthedocs.io/)
 
+## Usage
+
+Examples can be found in `example`.
+
+```python
+import matplotlib.pyplot as plt
+
+from bosing import Barrier, Channel, Hann, Play, Stack, generate_waveforms
+
+channels = [Channel("xy", 30e6, 2e9, 1000)]
+shapes = [Hann()]
+schedule = Stack(duration=500e-9).with_children(
+    Play(
+        channel_id=0,
+        shape_id=0,
+        amplitude=0.3,
+        width=100e-9,
+        plateau=200e-9,
+    ),
+    Barrier(duration=10e-9),
+)
+result = generate_waveforms(channels, shapes, schedule)
+w = result["xy"]
+plt.plot(w.real, label="I")
+plt.plot(w.imag, label="Q")
+plt.legend()
+plt.show()
+```
+
 ## Development
 
 ### Prerequisites
 
-* .NET 8 SDK. Install the latest .NET SDK from [here](https://dotnet.microsoft.com/download/dotnet) or install with Visual Studio.
+* Latest stable Rust toolchain.
+* [maturin](https://github.com/PyO3/maturin) 1.5+.
 * [hatch](https://github.com/pypa/hatch) for python project management.
 
 ### Development install
 
-Ensure `dotnet` cli is in `PATH`.
-
 ```bash
 git clone https://github.com/kahojyun/Bosing.git
 cd Bosing
 pip install -e .
 ```
 
 ### Build docs
@@ -36,42 +64,10 @@
 ```bash
 hatch run docs:build
 ```
 
 ### Run tests
 
 ```bash
-dotnet test
+cargo test
 hatch run test:run
 ```
-
-### Usage
-
-Examples can be found in `python/examples`.
-
-```python
-from bosing import Play, Barrier, Hann, Channel, Stack, generate_waveforms
-import matplotlib.pyplot as plt
-
-channels = [Channel("xy", 200e6, 2e9, 100000)]
-shapes = [Hann()]
-schedule = Stack(duration=50e-6).with_children(
-    Play(
-        channel_id = 0,
-        amplitude = 0.3,
-        shape_id = 0,
-        width = 100e-9,
-    ),
-    Barrier(duration=10e-9),
-)
-result = generate_waveforms(channels, shapes, schedule)
-i, q = result["xy"]
-plt.plot(i)
-plt.plot(q)
-plt.show()
-```
-
-### Tooling
-
-Use Visual Studio or Visual Studio Code with the [C# extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp).
-
-Manage python project with [hatch](https://github.com/pypa/hatch).
```

### Comparing `bosing-1.0.1/pyproject.toml` & `bosing-2.0.0b1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["maturin>=1.5,<2.0"]
+build-backend = "maturin"
 
 [project]
 name = "bosing"
 dynamic = ["version"]
 description = "Waveform generator for pulse sequences in quantum computing"
 readme = "README.md"
 requires-python = ">=3.8"
-license = "MIT"
 keywords = []
 authors = [{ name = "kaho", email = "kaho0769@qq.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
-    "Programming Language :: C#",
-    "Programming Language :: Python",
+    "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["numpy", "msgpack", "attrs"]
+dependencies = ["numpy"]
 
 [project.urls]
 Documentation = "https://github.com/kahojyun/Bosing#readme"
 Issues = "https://github.com/kahojyun/Bosing/issues"
 Source = "https://github.com/kahojyun/Bosing"
 
-[tool.hatch.version]
-path = "VERSION.txt"
-pattern = "(?P<version>.*)"
-
-[tool.hatch.build.hooks.custom]
-
-[tool.hatch.build.targets.wheel]
-packages = ["python/bosing"]
+[tool.maturin]
+features = ["pyo3/extension-module"]
 
 [tool.hatch.envs.default]
-dependencies = ["scipy", "matplotlib", "ipython"]
-
-[tool.hatch.envs.docs]
-dependencies = ["sphinx", "furo", "matplotlib"]
+dependencies = [
+    "maturin>=1.5,<2.0",
+    "scipy",
+    "matplotlib",
+    "ipython",
+    "sphinx",
+    "furo",
+    "mypy",
+]
 
-[tool.hatch.envs.docs.scripts]
-build = "sphinx-build -M html python/docs python/docs/_build {args}"
-clean = "rm -rf python/docs/_build docs/_autosummary"
+[tool.hatch.envs.default.scripts]
+mip = "maturin develop && ipython"
+stubcheck = "maturin develop && stubtest bosing --allowlist stubtest-allowlist.txt"
+build_docs = "maturin develop && sphinx-build -M html docs docs/_build {args}"
+clean_docs = "rm -rf docs/_build docs/generated"
 
-[tool.hatch.envs.docs.overrides]
+[tool.hatch.envs.default.overrides]
 platform.windows.scripts = [
-    'clean=rmdir /s /q python\\docs\\_build python\\docs\\_autosummary',
+    'clean_docs=rmdir /s /q docs\\_build docs\\generated',
 ]
 
 [tool.hatch.envs.test]
 dependencies = ["pytest"]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest {args}"
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
-testpaths = ["python/tests"]
+addopts = ["--import-mode=importlib"]
+testpaths = ["tests"]
 
 [tool.hatch.envs.hatch-static-analysis]
 config-path = "ruff_defaults.toml"
 
 [tool.ruff]
 extend = "ruff_defaults.toml"
-include = ["python/bosing/*.py", "python/tests/*.py"]
```

### Comparing `bosing-1.0.1/PKG-INFO` & `bosing-2.0.0b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 1.0.1
-Summary: Waveform generator for pulse sequences in quantum computing
-Project-URL: Documentation, https://github.com/kahojyun/Bosing#readme
-Project-URL: Issues, https://github.com/kahojyun/Bosing/issues
-Project-URL: Source, https://github.com/kahojyun/Bosing
-Author-email: kaho <kaho0769@qq.com>
-License-Expression: MIT
-License-File: LICENSE.txt
+Version: 2.0.0b1
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: C#
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Requires-Dist: attrs
-Requires-Dist: msgpack
+Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
-Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Summary: Waveform generator for pulse sequences in quantum computing
+Keywords: 
+Author-email: kaho <kaho0769@qq.com>
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Documentation, https://github.com/kahojyun/Bosing#readme
+Project-URL: Issues, https://github.com/kahojyun/Bosing/issues
+Project-URL: Source, https://github.com/kahojyun/Bosing
 
 # Bosing
 
 [![Documentation Status](https://readthedocs.org/projects/bosing/badge/?version=latest)](https://bosing.readthedocs.io/zh-cn/latest/?badge=latest)
 
 Waveform generator for superconducting circuits.
 
@@ -34,25 +32,53 @@
 pip install bosing
 ```
 
 ## Documentation
 
 Docs are hosted on [Read the Docs](http://bosing.readthedocs.io/)
 
+## Usage
+
+Examples can be found in `example`.
+
+```python
+import matplotlib.pyplot as plt
+
+from bosing import Barrier, Channel, Hann, Play, Stack, generate_waveforms
+
+channels = [Channel("xy", 30e6, 2e9, 1000)]
+shapes = [Hann()]
+schedule = Stack(duration=500e-9).with_children(
+    Play(
+        channel_id=0,
+        shape_id=0,
+        amplitude=0.3,
+        width=100e-9,
+        plateau=200e-9,
+    ),
+    Barrier(duration=10e-9),
+)
+result = generate_waveforms(channels, shapes, schedule)
+w = result["xy"]
+plt.plot(w.real, label="I")
+plt.plot(w.imag, label="Q")
+plt.legend()
+plt.show()
+```
+
 ## Development
 
 ### Prerequisites
 
-* .NET 8 SDK. Install the latest .NET SDK from [here](https://dotnet.microsoft.com/download/dotnet) or install with Visual Studio.
+* Latest stable Rust toolchain.
+* [maturin](https://github.com/PyO3/maturin) 1.5+.
 * [hatch](https://github.com/pypa/hatch) for python project management.
 
 ### Development install
 
-Ensure `dotnet` cli is in `PATH`.
-
 ```bash
 git clone https://github.com/kahojyun/Bosing.git
 cd Bosing
 pip install -e .
 ```
 
 ### Build docs
@@ -60,42 +86,11 @@
 ```bash
 hatch run docs:build
 ```
 
 ### Run tests
 
 ```bash
-dotnet test
+cargo test
 hatch run test:run
 ```
 
-### Usage
-
-Examples can be found in `python/examples`.
-
-```python
-from bosing import Play, Barrier, Hann, Channel, Stack, generate_waveforms
-import matplotlib.pyplot as plt
-
-channels = [Channel("xy", 200e6, 2e9, 100000)]
-shapes = [Hann()]
-schedule = Stack(duration=50e-6).with_children(
-    Play(
-        channel_id = 0,
-        amplitude = 0.3,
-        shape_id = 0,
-        width = 100e-9,
-    ),
-    Barrier(duration=10e-9),
-)
-result = generate_waveforms(channels, shapes, schedule)
-i, q = result["xy"]
-plt.plot(i)
-plt.plot(q)
-plt.show()
-```
-
-### Tooling
-
-Use Visual Studio or Visual Studio Code with the [C# extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp).
-
-Manage python project with [hatch](https://github.com/pypa/hatch).
```

