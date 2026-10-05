<!-- SPDX-FileCopyrightText: Cadasto B.V. -->
<!-- SPDX-License-Identifier: BUSL-1.1 -->
# <img src="assets/brand/ferrotask-icon.svg" alt="" width="40" height="40" align="top"> FerroTASK

[![License: BUSL-1.1](https://img.shields.io/badge/License-BUSL--1.1-blue.svg)](LICENSE)

The task planning and decision support server for the openEHR platform, in pure Rust: what happens next.

A record says what has happened to a patient. A care pathway says what should happen next, who does it, and what to decide when a result comes in. FerroTASK runs that half. It executes task plans written to the openEHR Task Planning specification, from the [Process (PROC)](https://specifications.openehr.org/releases/PROC/development) component, and evaluates the rules in them with the Decision Language. It also evaluates guidelines written in GDL2, from the [Clinical Decision Support (CDS)](https://specifications.openehr.org/releases/CDS/development) component. Both read the patient's data by archetype and template path, so FerroTASK reads from and commits to an openEHR CDR such as FerroEHR and holds no clinical record of its own.

FerroTASK is one of the [FerroHEALTH](https://ferrohealth.eu/) family. The family
page shows where it sits among the products and what calls what, and this
repository is where the design and the build happen; the tracker is the
record of both. Its site will be <https://ferrotask.eu/>.

## Licence

FerroTASK is source-available under the Business Source License 1.1. The
parameters that apply, the Licensor, the Licensed Work, the Additional Use
Grant and the Change Date, are in [LICENSE](LICENSE): free for non-commercial
production use, a commercial licence for any other production use, and Apache
2.0 four years after each version is published. The maintainer named in
[MAINTAINERS.md](MAINTAINERS.md) is the contact for a commercial licence.

The brand assets under `assets/brand/` are part of the Licensed Work.

Contributions carry the terms in
[CONTRIBUTING.md](CONTRIBUTING.md#licensing-of-contributions): you keep your
copyright, and you grant the Licensor the relicensing right that keeps the work
one work under one licensor. There is no separate agreement to sign.
