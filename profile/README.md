<a href="https://www.jku.at/en/institute-for-integrated-circuits-and-quantum-computing/">
  <img src="https://raw.githubusercontent.com/iic-jku/.github/main/profile/fig/iic-jku.svg" alt="Johannes Kepler University: Institute for Integrated Circuits and Quantum Computing" width="50%"/>
</a>

# Institute for Integrated Circuits and Quantum Computing (IICQC) at the Johannes Kepler University Linz (JKU)

We build open-source tools, chip design templates with tutorials, course material and complete chip designs for the open-source PDKs from IHP, SkyWater and GlobalFoundries. Everything here is regression-tested against the latest tool versions. Visit us [here](https://www.jku.at/en/institute-for-integrated-circuits-and-quantum-computing/).

**[Tools](#tools)** · **[Templates & Tutorials](#templates--tutorials)** · **[Courses](#courses)** · **[Open Chip Projects](#open-chip-projects)** · **[Chip Gallery](#chip-gallery)** · **[Regression Tests](#regression-tests)** · **[More](#more)**

## Tools

| Tool | What it does | Links |
| ---- | ------------ | ----- |
| [**IIC-OSIC-TOOLS**](https://github.com/iic-jku/IIC-OSIC-TOOLS) | All-in-one Docker image for open-source analog and digital chip design with the SKY130, GF180 and IHP 130 nm PDKs, native on AMD64 and ARM64 | [Docker Hub](https://hub.docker.com/r/hpretl/iic-osic-tools) · [Zenodo](https://doi.org/10.5281/zenodo.14387234) |
| [**KPEX**](https://github.com/iic-jku/klayout-pex) | Parasitic extraction for KLayout, with plugins for the FEM field solvers [gmsh](https://github.com/iic-jku/klayout-pex-plugin-gmsh), [Palace](https://github.com/iic-jku/klayout-pex-plugin-palace), [Elmer](https://github.com/iic-jku/klayout-pex-plugin-elmer) and [KQCircuits](https://github.com/iic-jku/klayout-pex-plugin-kqcircuits) | [Docs](https://iic-jku.github.io/klayout-pex-website/) · [PyPI](https://pypi.org/project/klayout-pex/) · [Zenodo](https://doi.org/10.5281/zenodo.17822625) |
| [**KLayout Productivity Suite**](https://github.com/iic-jku/klayout-productivity-suite) | KLayout plugins for aligning, moving, pins, layer shortcuts, auto backup, library management, netlist import and PDF/SVG export, installed as one package from the KLayout package manager | [Docs](https://iic-jku.github.io/klayout-productivity-suite/) · [Zenodo](https://doi.org/10.5281/zenodo.17822158) |
| [**snp2le**](https://github.com/iic-jku/snp2le) | Converts Touchstone S-parameter files into lumped-element netlists for ngspice, VACASK and Xyce (GUI and CLI) | [PyPI](https://pypi.org/project/snp2le/) · [Zenodo](https://doi.org/10.5281/zenodo.21189545) |
| [**chipify**](https://github.com/iic-jku/chipify) | Automates mismatch and Monte-Carlo simulations, parameter sweeps and yield analysis with Xschem and ngspice (GUI and CLI) | [chipify.io](https://chipify.io/) · [PyPI](https://pypi.org/project/chipify/) · [Examples](https://github.com/iic-jku/chipify-examples) |
| [**PREP-IC**](https://github.com/iic-jku/prep-ic) | Pinout, Ring and Early floorplan Planner for ICs: plans pad rings and pinouts with live die sizing and RF/GSG pad groups (GUI and Python API) | [PyPI](https://pypi.org/project/prep-ic/) · [Zenodo](https://doi.org/10.5281/zenodo.23963620) |

## Templates & Tutorials

Our analog mixed-signal (AMS) chip templates take a design from the specification to a tapeout-ready chip. Inside IIC-OSIC-TOOLS, `make all` runs the simulations, hardens the digital macros, generates the padframe, assembles the top level and verifies the chip with DRC, LVS and PEX. Each template comes with a step-by-step tutorial.

| PDK | Template | Links |
| --- | -------- | ----- |
| IHP SG13G2 (130 nm BiCMOS) | [ihp-sg13g2-ams-chip-template](https://github.com/iic-jku/ihp-sg13g2-ams-chip-template) | [Tutorial](https://iic-jku.github.io/ihp-sg13g2-ams-chip-template/) · [Zenodo](https://doi.org/10.5281/zenodo.20129233) |
| IHP SG13CMOS5L (130 nm CMOS) | [ihp-sg13cmos5l-ams-chip-template](https://github.com/iic-jku/ihp-sg13cmos5l-ams-chip-template) | [Tutorial](https://iic-jku.github.io/ihp-sg13cmos5l-ams-chip-template/) · [Zenodo](https://doi.org/10.5281/zenodo.22115134) |
| SkyWater SKY130A (130 nm) | [sky130A-ams-chip-template](https://github.com/iic-jku/sky130A-ams-chip-template) *(public soon)* | [Tutorial](https://iic-jku.github.io/sky130A-ams-chip-template/) *(public soon)* |
| GlobalFoundries GF180MCU-D (180 nm) | [gf180mcuD-ams-chip-template](https://github.com/iic-jku/gf180mcuD-ams-chip-template) *(public soon)* | [Tutorial](https://iic-jku.github.io/gf180mcuD-ams-chip-template/) *(public soon)* |

## Courses

Material of our lectures at JKU, free to read online.

| Course | Level | JKU course | Material |
| ------ | ----- | ---------- | -------- |
| **Analog (Integrated) Circuit Design** | Intermediate | 336.009 | [Online](https://iic-jku.github.io/analog-circuit-design/aicd.html) · [Repository](https://github.com/iic-jku/analog-circuit-design) · [Zenodo](https://doi.org/10.5281/zenodo.14387481) |
| **Radio-Frequency Integrated Circuits** | Graduate | 336.023 | [Online](https://iic-jku.github.io/radio-frequency-integrated-circuits/rfic.html) · [Repository](https://github.com/iic-jku/radio-frequency-integrated-circuits) · [Zenodo](https://doi.org/10.5281/zenodo.17563943) |
| **Design of Complex Integrated Circuits** | Graduate | 336.048 | [Online](https://iic-jku.github.io/design-complex-ic/dcic.html) · [Repository](https://github.com/iic-jku/design-complex-ic) |
| **VLSI Design** | Graduate | 336.051 | [Online](https://iic-jku.github.io/vlsi-design/vlsi.html) · [Repository](https://github.com/iic-jku/vlsi-design) |

## Open Chip Projects

Complete chip designs with all design data, simulations and documentation. Both are built on the [ihp-sg13g2-ams-chip-template](https://github.com/iic-jku/ihp-sg13g2-ams-chip-template) and were taped out on an IHP MPW in March 2026.

| Project | Description | Links |
| ------- | ----------- | ----- |
| [**TinyWhisper**](https://github.com/iic-jku/TinyWhisper) | Fully integrated multi-mode short-wave transmitter for amateur radio in 130 nm CMOS, designed together with JMU Würzburg | [Docs](https://iic-jku.github.io/TinyWhisper/) · [Zenodo](https://doi.org/10.5281/zenodo.20004085) |
| [**SPARX**](https://github.com/iic-jku/SG13CMOS_SPARX) | Automated, programmatically generated, frequency-scalable six-port receiver in 130 nm CMOS, with EM simulations in AWS Palace | [Docs](https://iic-jku.github.io/SG13CMOS_SPARX/) · [Zenodo](https://doi.org/10.5281/zenodo.19654232) |

## Chip Gallery

The [Open-Source Chip Gallery](https://github.com/iic-jku/open-source-chip-gallery) collects the chips we designed and taped out, each with its final layout, rendered layout images and a link to the full design data. The latest entries:

| Chip | Technology | Shuttle | Tapeout |
| ---- | ---------- | ------- | ------- |
| [SPARX](https://github.com/iic-jku/open-source-chip-gallery#sparx-ihp-mpw-tapeout) | IHP SG13CMOS (130 nm) | IHP MPW | March 2026 |
| [TinyWhisper](https://github.com/iic-jku/open-source-chip-gallery#tinywhisper-ihp-mpw-tapeout) | IHP SG13CMOS (130 nm) | IHP MPW | March 2026 |
| [Multi-Project Chip](https://github.com/iic-jku/open-source-chip-gallery#multi-project-chip-waferspace) | GF180MCU (180 nm) | wafer.space run 1 | December 2025 |
| [IQ Modulator](https://github.com/iic-jku/open-source-chip-gallery#iq-modulator-tiny-tapeout) | SkyWater SKY130A (130 nm) | Tiny Tapeout ttsky25b | November 2025 |

## Regression Tests

We test on two levels. Every repository runs its own CI, and the nightly build of IIC-OSIC-TOOLS runs integration tests that clone our templates, chip projects and courses, so a tool update that breaks one of them shows up the next morning.

### Repository CI

The Status column shows the latest result of each repository's own CI workflow, run on the branch given. The image column names the IIC-OSIC-TOOLS container the workflow runs in: `latest` is the most recent release (`hpretl/iic-osic-tools:latest`), `nightly` is the image of the last nightly build (`ghcr.io/iic-jku/iic-osic-tools:nightly`), and none means the workflow installs its tools itself.

<!--
When the sky130A and gf180mcuD templates go public, replace their "(public soon)" status cells with:
[![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/sky130A-ams-chip-template/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/sky130A-ams-chip-template/actions/workflows/regression.yml)
[![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/gf180mcuD-ams-chip-template/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/gf180mcuD-ams-chip-template/actions/workflows/regression.yml)

When open-pdks-regression-tests PR #12 is merged, replace its status cell with:
[![ihp-sg13g2](https://img.shields.io/github/actions/workflow/status/iic-jku/open-pdks-regression-tests/regression-ihp-sg13g2.yml?branch=main&label=ihp-sg13g2)](https://github.com/iic-jku/open-pdks-regression-tests/actions/workflows/regression-ihp-sg13g2.yml) [![ihp-sg13cmos5l](https://img.shields.io/github/actions/workflow/status/iic-jku/open-pdks-regression-tests/regression-ihp-sg13cmos5l.yml?branch=main&label=ihp-sg13cmos5l)](https://github.com/iic-jku/open-pdks-regression-tests/actions/workflows/regression-ihp-sg13cmos5l.yml) [![gf180mcuD](https://img.shields.io/github/actions/workflow/status/iic-jku/open-pdks-regression-tests/regression-gf180mcuD.yml?branch=main&label=gf180mcuD)](https://github.com/iic-jku/open-pdks-regression-tests/actions/workflows/regression-gf180mcuD.yml) [![sky130A](https://img.shields.io/github/actions/workflow/status/iic-jku/open-pdks-regression-tests/regression-sky130A.yml?branch=main&label=sky130A)](https://github.com/iic-jku/open-pdks-regression-tests/actions/workflows/regression-sky130A.yml)
-->

| Repository | What runs | Trigger | Branch | IIC-OSIC-TOOLS image | Status |
| ---------- | --------- | ------- | ------ | -------------------- | ------ |
| [IIC-OSIC-TOOLS](https://github.com/iic-jku/IIC-OSIC-TOOLS) | Nightly image build with the latest tool versions and 48 integration tests on AMD64 and ARM64 (see [below](#iic-osic-tools-nightly-regression)) | Sunday to Thursday at 23:00 UTC, skipped when nothing changed since the last green night (at least every 6 days), manual | `next_release` | `nightly`, built in the same run | [![nightly](https://img.shields.io/github/actions/workflow/status/iic-jku/IIC-OSIC-TOOLS/nightly.yaml?branch=main&label=nightly)](https://github.com/iic-jku/IIC-OSIC-TOOLS/actions/workflows/nightly.yaml) |
| [open-pdks-regression-tests](https://github.com/iic-jku/open-pdks-regression-tests) | One workflow per PDK (ihp-sg13g2, ihp-sg13cmos5l, gf180mcuD, sky130A): `make regression` (DRC, LVS and PEX), then `make pex-bench` | Push and pull request (documentation changes excepted), manual | `main` | `nightly` (selectable in a manual run) | *(coming with [#12](https://github.com/iic-jku/open-pdks-regression-tests/pull/12))* |
| [ihp-sg13g2-ams-chip-template](https://github.com/iic-jku/ihp-sg13g2-ams-chip-template) | `make regression`: full chip build with DRC, LVS and PEX | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | [![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/ihp-sg13g2-ams-chip-template/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/ihp-sg13g2-ams-chip-template/actions/workflows/regression.yml) |
| [ihp-sg13cmos5l-ams-chip-template](https://github.com/iic-jku/ihp-sg13cmos5l-ams-chip-template) | `make regression`: full chip build with DRC, LVS and PEX | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | [![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/ihp-sg13cmos5l-ams-chip-template/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/ihp-sg13cmos5l-ams-chip-template/actions/workflows/regression.yml) |
| [sky130A-ams-chip-template](https://github.com/iic-jku/sky130A-ams-chip-template) *(public soon)* | `make regression`: full chip build with DRC, LVS and PEX | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | *(public soon)* |
| [gf180mcuD-ams-chip-template](https://github.com/iic-jku/gf180mcuD-ams-chip-template) *(public soon)* | `make regression`: full chip build with DRC, LVS and PEX | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | *(public soon)* |
| [TinyWhisper](https://github.com/iic-jku/TinyWhisper) | `make regression-nightly`: full chip build and verification | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | [![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/TinyWhisper/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/TinyWhisper/actions/workflows/regression.yml) |
| [SPARX](https://github.com/iic-jku/SG13CMOS_SPARX) | `make regression-nightly`: full chip build and verification, including the GDSFactory flows | Daily at 02:00 UTC when `main` changed in the last 25 hours, manual | `main` | `latest` | [![regression](https://img.shields.io/github/actions/workflow/status/iic-jku/SG13CMOS_SPARX/regression.yml?branch=main&label=regression)](https://github.com/iic-jku/SG13CMOS_SPARX/actions/workflows/regression.yml) |
| [Analog Circuit Design](https://github.com/iic-jku/analog-circuit-design) | Simulation of the Xschem testbenches and execution of the gm/ID notebooks | Push and pull request that change the tested files, manual | `main` | `latest` (simulations), none (notebooks) | [![simulation](https://img.shields.io/github/actions/workflow/status/iic-jku/analog-circuit-design/simulation-test.yml?branch=main&label=simulation)](https://github.com/iic-jku/analog-circuit-design/actions/workflows/simulation-test.yml) [![notebooks](https://img.shields.io/github/actions/workflow/status/iic-jku/analog-circuit-design/notebook-test.yml?branch=main&label=notebooks)](https://github.com/iic-jku/analog-circuit-design/actions/workflows/notebook-test.yml) |
| [VLSI Design](https://github.com/iic-jku/vlsi-design) | Checks of the course examples, chapter by chapter | Push and pull request that change the tested files, manual | `main` | `latest` (selectable in a manual run) | [![checks](https://img.shields.io/github/actions/workflow/status/iic-jku/vlsi-design/course-checks.yml?branch=main&label=checks)](https://github.com/iic-jku/vlsi-design/actions/workflows/course-checks.yml) |
| [KPEX](https://github.com/iic-jku/klayout-pex) | Multi-platform build and tests | Push, pull request and release | `main`, `next_release` | none | [![tests](https://img.shields.io/github/actions/workflow/status/iic-jku/klayout-pex/ci-cd.yml?branch=main&event=push&label=tests)](https://github.com/iic-jku/klayout-pex/actions/workflows/ci-cd.yml) |
| [snp2le](https://github.com/iic-jku/snp2le) | Unit and GUI tests | Push and pull request | `main` | none | [![tests](https://img.shields.io/github/actions/workflow/status/iic-jku/snp2le/tests.yml?branch=main&label=tests)](https://github.com/iic-jku/snp2le/actions/workflows/tests.yml) |
| [chipify](https://github.com/iic-jku/chipify) | Unit tests | Push and pull request | `master` | none | [![tests](https://img.shields.io/github/actions/workflow/status/iic-jku/chipify/ci.yml?branch=master&label=tests)](https://github.com/iic-jku/chipify/actions/workflows/ci.yml) |
| [PREP-IC](https://github.com/iic-jku/prep-ic) | Unit and GUI tests | Push and pull request | `main` | none | [![tests](https://img.shields.io/github/actions/workflow/status/iic-jku/prep-ic/tests.yml?branch=main&label=tests)](https://github.com/iic-jku/prep-ic/actions/workflows/tests.yml) |

### IIC-OSIC-TOOLS Nightly Regression

Every night from Sunday to Thursday, IIC-OSIC-TOOLS builds its `next_release` branch with the latest tool versions as `ghcr.io/iic-jku/iic-osic-tools:nightly` and runs the [48 integration tests](https://github.com/iic-jku/IIC-OSIC-TOOLS/blob/next_release/_tests/TESTS.md) on AMD64 and ARM64. These tests clone our other repositories at the branch given here:

| Repository | Branch | Tests |
| ---------- | ------ | ----- |
| [ihp-sg13g2-ams-chip-template](https://github.com/iic-jku/ihp-sg13g2-ams-chip-template) | `next_release` | 20: `make regression` |
| [ihp-sg13cmos5l-ams-chip-template](https://github.com/iic-jku/ihp-sg13cmos5l-ams-chip-template) | `next_release` | 32: `make regression` |
| [TinyWhisper](https://github.com/iic-jku/TinyWhisper) | `next_release` | 28: `make regression` |
| [SPARX](https://github.com/iic-jku/SG13CMOS_SPARX) | `next_release` | 22: `make regression` |
| [VLSI Design](https://github.com/iic-jku/vlsi-design) | `next_release` | 49: course examples (lint, simulation, synthesis, STA, DFT, LibreLane) |
| [Analog Circuit Design](https://github.com/iic-jku/analog-circuit-design) | `main` | 21: xschem/ngspice simulation testbenches |
| [open-pdks-regression-tests](https://github.com/iic-jku/open-pdks-regression-tests) | `main` | 26, 31, 47, 48: DRC, LVS and PEX for each PDK, 35: PEX bench |

The PDK coverage of the nightly regression, by test ID:

| Area | sky130A | gf180mcuD | ihp-sg13g2 | ihp-sg13cmos5l |
| ---- | :-----: | :-------: | :--------: | :------------: |
| Digital flow (LibreLane, ORFS) | 01, 07 | 04 | 10, 18 | 19 |
| Analog simulation (ngspice, Xyce, VACASK) | 06 | 14 | 05, 11, 36, 45 | 29, 36 |
| EM simulation (Palace) | – | – | 43 | – |
| DRC, LVS and PEX | 02, 23–25 | 23–25 | 23–25 | 23–25 |
| KLayout PCells, standard cells and GUI DRC/LVS | 27 | 27 | 27, 34, 38 | 27, 34, 38 |
| open-pdks regression (DRC, LVS, PEX) | 48 | 47 | 26 | 31 |
| open-pdks PEX bench (Magic, KPEX) | 35 | 35 | 35 | 35 |
| AMS chip template | – | – | 20 | 32 |
| Chip projects | – | – | 22 (SPARX), 28 (TinyWhisper) | – |
| Courses | – | – | – | 21 (Analog Circuit Design), 49 (VLSI Design) |

Further tests cover PDK-independent tools, such as the Python packages, the RISC-V toolchain, Chisel, Veryl, Verilator with UVM and FST tracing, FPGA flows, KQCircuits and mixed-signal co-simulation.

## More

- [Harald Pretl's lectures](https://github.com/iic-jku/hpretl-lectures): collected lectures on integrated circuit design
- [Fifty Nifty Variations of Two-Transistor Circuits](https://iic-jku.github.io/fifty-nifty-circuits/): paper and posters, also as a web edition ([Zenodo](https://doi.org/10.5281/zenodo.15016440))
- [Circuit Designer's Etiquette](https://github.com/iic-jku/Circuit-Designers-Etiquette): rules and recommendations for analog and digital circuit designers
- [Microelectronics in Austria](https://iic-jku.github.io/map-microelectronics-austria/): interactive map of the Austrian microelectronics ecosystem
- [iic-circdia](https://github.com/iic-jku/iic-circdia): our LaTeX package for circuit diagrams

_Most of our later work on quantum computing can be found at [cda-tum](https://github.com/cda-tum)._
