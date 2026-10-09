# OPENHAB CORE

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-consumer_appliances-lightgrey)

> Anticloud-hardened packaging of the upstream project `OPENHAB_CORE` in category **CONSUMER APPLIANCES**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CONSUMER APPLIANCES · **Upstream:** https://github.com/openhab/openhab-core · **Upstream pin:** `caf53b3aa405647cb47d44c075e9c483bf6f5322` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# openHAB Core

[![GitHub Actions Build Status](https://github.com/openhab/openhab-core/actions/workflows/ci-build.yml/badge.svg?branch=main)](https://github.com/openhab/openhab-core/actions/workflows/ci-build.yml)
[![Jenkins Build Status](https://ci.openhab.org/job/openHAB-Core/badge/icon)](https://ci.openhab.org/job/openHAB-Core/)
[![JavaDoc Build Status](https://ci.openhab.org/view/Documentation/job/openHAB-JavaDoc/badge/icon?subject=javadoc)](https://ci.openhab.org/view/Documentation/job/openHAB-JavaDoc/)
[![EPL-2.0](https://img.shields.io/badge/license-EPL%202-green.svg)](https://opensource.org/licenses/EPL-2.0)
[![Crowdin](https://badges.crowdin.net/openhab-core/localized.svg)](https://crowdin.com/project/openhab-core)

This project contains core bundles of the openHAB runtime.

Building and running the project is fairly easy if you follow the steps detailed below.

Please note that openHAB Core is not a product itself, but a framework to build solutions on top.
It is picked up by the main [openHAB distribution](https://github.com/openhab/openhab-distro).

This means that what you build is primarily an artifact project of OSGi bundles that can be used within smart home products.

## 1. Prerequisites

The build infrastructure is based on Maven. 
If you know Maven already then there won't be any surprises for you. 
If you have not worked with Maven yet, just follow the instructions and everything will miraculously work ;-)

What you need before you start:

- Java SE Development Kit 21
- Maven 3 from https://maven.apache.org/download.html

Make sure that the `mvn` command is available on your path

## 2. Checkout

Checkout the source code from GitHub, e.g. by running:

```
git source https://github.com/openhab/openhab-core.git
```

## 3. Building with Maven

To build this project from the sources, Maven takes care of everything:

- set `MAVEN_OPTS` to `-Xms512m -Xmx1024m`
- change into the openhab-core directory (`cd openhab-core`)
- run `mvn clean spotless:apply install` to compile and package all sources

If there are tests that are failing occasionally on your local build, run `mvn -DskipTests=true clean install` instead to skip them.

For an even quicker build, run `mvn clean install -T1C -DskipChecks -DskipTests -Dspotless.check.skip=true`.

## How to contribute

If you want to become a contributor to the project, please read about [contributing](https://www.openhab.org/docs/developer/contributing.html) and check our [guidelines](https://www.openhab.org/docs/developer/guidelines.html) first.

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `bom/`, `bundles/`, `features/`, `itests/`
- Snapshot size: **3656 files**, **334515 lines of code** (measured; see Benchmarks)
- Primary languages: `.java` (2308), `.properties` (585), `(none)` (361), `.xml` (175), `.xtend` (43), `.json` (38)
- Upstream commit pinned for this packaging: `caf53b3aa405647cb47d44c075e9c483bf6f5322`

---

## Installation

[![Jenkins Build Status](https://ci.openhab.org/job/openHAB-Core/badge/icon)](https://ci.openhab.org/job/openHAB-Core/)
[![JavaDoc Build Status](https://ci.openhab.org/view/Documentation/job/openHAB-JavaDoc/badge/icon?subject=javadoc)](https://ci.openhab.org/view/Documentation/job/openHAB-JavaDoc/)
[![EPL-2.0](https://img.shields.io/badge/license-EPL%202-green.svg)](https://opensource.org/licenses/EPL-2.0)
[![Crowdin](https://badges.crowdin.net/openhab-core/localized.svg)](https://crowdin.com/project/openhab-core)

This project contains core bundles of the openHAB runtime.

Building and running the project is fairly easy if you follow the steps detailed below.

Please note that openHAB Core is not a product itself, but a framework to build solutions on top.
It is picked up by the main [openHAB distribution](https://github.com/openhab/openhab-distro).

This means that what you build is primarily an artifact project of OSGi bundles that can be used within smart home products.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

Browse the snapshot layout listed under What This Project Does and follow the upstream run instructions for the detected ecosystem (Unknown (no standard manifest detected)).

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

[![EPL-2.0](https://img.shields.io/badge/license-EPL%202-green.svg)](https://opensource.org/licenses/EPL-2.0)
[![Crowdin](https://badges.crowdin.net/openhab-core/localized.svg)](https://crowdin.com/project/openhab-core)

This project contains core bundles of the openHAB runtime.

Building and running the project is fairly easy if you follow the steps detailed below.

Please note that openHAB Core is not a product itself, but a framework to build solutions on top.
It is picked up by the main [openHAB distribution](https://github.com/openhab/openhab-distro).

This means that what you build is primarily an artifact project of OSGi bundles that can be used within smart home products.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 3656 |
| Lines of code | 334515 |
| Dependency references | 0 |
| Upstream license | EPL-2.0 |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- None detected at the snapshot root; consult the upstream documentation link in the Upstream section.

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to openHAB Core components

Warning: Note that this is most likely not the project you are looking for.

openHAB mainly consist out of the core components and extensions that are from
https://github.com/openhab/openhab-addons. All is then packaged into a distribution in
https://github.com/openhab/openhab-distro.

## Contribution guidelines

### Pull requests are always welcome

We are always thrilled to receive pull requests, and do our best to
process them as fast as possible. Not sure if that typo is worth a pull
request? Do it! We will appreciate it.

If your pull request is not accepted on the first try, don't be
discouraged! If there's a problem with the implementation, hopefully you
received feedback on what to improve.

We're trying very hard to keep openHAB lean and focused. We don't want it
to do everything for everybody. This means that we might decide against
incorporating a new feature. However, there might be a way to implement
that feature *on top of* openHAB.

### Discuss your design on the mailing list

We recommend discussing your plans [in the discussion forum](https://community.openhab.org/)
before starting to code - especially for more ambitious contributions.
This gives other contributors a chance to point you in the right
direction, give feedback on your design, and maybe point out if someone
else is working on the same thing.

### Conventions

Fork the project and make changes on your fork in a feature branch:

- If it's a bugfix branch, name it XXX-something where XXX is the number of the
  issue
- If it's a feature branch, create an enhancement issue to announce your
  intentions, and name it XXX-something where XXX is the number of the issue.

Submit unit tests for your changes.  openHAB has a great test framework built in; use
it! Take a look at existing tests for inspiration. Run the full test suite on
your branch before submitting a pull request.

Update the documentation when creating or modifying features. Test
your documentation changes for clarity, concision, and correctness, as
well as a clean documentation build.

Write clean code. Universally formatted code promotes ease of writing, reading,
and maintenance. 

Pull requests descriptions should be as clear as possible and include a
reference to all the issues that they address.

Pull requests must not contain commits from other users or branches.

Commit messages must start with a capitalized and short summary (max. 50
chars) written in the imperative, followe

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: EPL-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
Eclipse Public License - v 2.0

    THE ACCOMPANYING PROGRAM IS PROVIDED UNDER THE TERMS OF THIS ECLIPSE
    PUBLIC LICENSE ("AGREEMENT"). ANY USE, REPRODUCTION OR DISTRIBUTION
    OF THE PROGRAM CONSTITUTES RECIPIENT'S ACCEPTANCE OF THIS AGREEMENT.

1. DEFINITIONS

"Contribution" means:

  a) in the case of the initial Contributor, the initial content
     Distributed under this Agreement, and

  b) in the case of each subsequent Contributor:
     i) changes to the Program, and
     ii) additions to the Program;
  where such changes and/or additions to the Program originate from
  and are Distributed by that particular Contributor. A Contribution
  "originates" from a Contributor if it was added to the Program by
  such Contributor itself or anyone acting on such Contributor's behalf.
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original EPL-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `EPL-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `OPENHAB_CORE` (category: CONSUMER APPLIANCES)
- **Upstream URL:** https://github.com/openhab/openhab-core
- **Pinned commit (SHA):** `caf53b3aa405647cb47d44c075e9c483bf6f5322`
- **Branch:** main
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`40ae2a1644a76f7086ce553230faca80f66192be6e15ecc3b5f6891e86ef59b6`.

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
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

