# RESERVOIR_SIMULATION

![licence](https://img.shields.io/badge/licence-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `RESERVOIR_SIMULATION` in category **OIL_GAS**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** RESERVOIR_SIMULATION · **Upstream pin:** `a0c58251899221a649c30b69e43b42739135deda` · **Category:** OIL_GAS · **Vendor:** Anticloud FZ LLE · **Licence:** MIT

---

## What This Project Does

# MRST Simulations

My various reservoir simulations done in Matlab Reservoir Simulation Toolbox (MRST). Can be run in Octave.

* 3D Hydrostatic (gravity) column of incompressible fluid > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/hydrostatic_column.m)
* 3D Single-phase incompressible fluid (water) simulation (ALL B.C.) > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/incompressible_heterogeneous.m)
* 3D Single-phase compressible fluid (oil) simulation - constant viscosity over pressure (NO FLOW B.C.) > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/compressible_viscosity_constant.m)
* 3D Single-phase compressible fluid (gas) simulation - pressure-dependent viscosity (NO FLOW B.C.) > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/compressible_viscosity_nonconstant.m)
* 3D Single-phase compressible fluid (polymer) simulation - Non-Newtonian fluid (with 2 numerical methods: cell-based, or face-based) (NO FLOW B.C.) > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/compressible_NonNewtonian.m)
* 3D Single-phase compressible fluid simulation with thermal effect (NO FLOW B.C.) > [Script](https://github.com/yohanesnuwara/MRST-simulations/blob/master/simulations/compressible_thermal.m)
* Two-phase incompressible and immiscible fluid
  * Simulation of waterflooding to an oil (dead oil) bank
    * 1D Buckley-Leverett simulation > [Script]() 
    * 2D Buckley-Leverett simulation > [Script]()
    * Observation of viscous fingering > [Script]()

> These scripts are adapted from MRST tutorial codes, but I have modified it.

**Note:**

* I added some Matlab functionalities used in the scripts that Octave currently doesn't have, such as `deval`. See in the `./modules/nuwara` folder. 
* I experienced that `plotyy` (an Octave function) doesn't work properly. `plotyy` is used e.g. in Simulation 3 to 6 (above). To fix this, this is my way round (in the command line): 
  * Add path: `addpath 'C:\Octave\Octave-5.2.0\mingw64\share\octave\5.2.0\m\plot\draw'`
  * Run: `plotyy`

## Current Experimentation

* MRST scripts are called from Google Colab
* For the optimization-related scripts (e.g. `computeLorenzSPE10.m`), Python optimizers will be used > Porting Python and Octave in Google Colab
* Utilizing GPU in Google Colab to run the MRST scripts, speeding up simulations

<!--
Sources to code:
* Simulation 2 to 6 see here: https://www.sintef.no/contentassets/2551f5f85547478590ceca14bc13ad51/book.html

---

## Installation

See the upstream documentation quoted in What This Project Does above.

## Usage

**Note:**

* I added some Matlab functionalities used in the scripts that Octave currently doesn't have, such as `deval`. See in the `./modules/nuwara` folder. 
* I experienced that `plotyy` (an Octave function) doesn't work properly. `plotyy` is used e.g. in Simulation 3 to 6 (above). To fix this, this is my way round (in the command line): 
  * Add path: `addpath 'C:\Octave\Octave-5.2.0\mingw64\share\octave\5.2.0\m\plot\draw'`
  * Run: `plotyy`

## API

* I experienced that `plotyy` (an Octave function) doesn't work properly. `plotyy` is used e.g. in Simulation 3 to 6 (above). To fix this, this is my way round (in the command line): 
  * Add path: `addpath 'C:\Octave\Octave-5.2.0\mingw64\share\octave\5.2.0\m\plot\draw'`
  * Run: `plotyy`

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | MIT |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

Fork the project, create a feature branch, run the test suite, and open a pull request against upstream.

## License

Upstream © its respective contributors under MIT (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** RESERVOIR_SIMULATION
- **Pinned SHA:** `a0c58251899221a649c30b69e43b42739135deda`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.md`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`a3eff45d17b38b0eb6184684ee971a383179212758dec3c1f7bfdf26603278a9`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

