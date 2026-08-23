# Antica Fiamma

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21479971.svg)](https://doi.org/10.5281/zenodo.21479971)

**Antica Fiamma (AF)** is a continuously updated, line-first research environment for Dante's *Commedia*, created and maintained by Ruoci Song. It reorganises commentary material from the Dartmouth Dante Project (DDP) into inspectable reading routes while keeping Dante's text, source commentary, and project-derived scholarly layers distinct.

- Live research environment: [https://anticafiamma.it](https://anticafiamma.it)
- Public code and documentation repository: [https://github.com/ruocisong/antica-fiamma-public](https://github.com/ruocisong/antica-fiamma-public)
- Archived release: [Antica Fiamma 1.0.0 on Zenodo](https://doi.org/10.5281/zenodo.21479971)
- Creator: [Ruoci Song](https://orcid.org/0009-0004-1263-2192), University of Bologna

The live site continues to change after the archived 1.0.0 release. Cite the Zenodo deposit when a stable software/documentation snapshot is required, and cite the live environment with an access date when referring to its current interface or runtime content.

## What Antica Fiamma Does

AF keeps the canto-line coordinate as an accountable scholarly anchor. Readers can move among:

- canto-level maps and line-level commentary coverage;
- source-attributed commentary cards and side-by-side comparison;
- Dante word-locus routes and cross-canto recurrence candidates;
- interpretive fields presented as derived, inspectable reading aids;
- author, work, and personaggio pathways in the Authority Layer;
- versioned research rooms, beginning with the Fiamma room on Dante's fire vocabulary.

The public build documented for version 1.0.0 mounts all 100 cantos and reports 14,233 line profiles, 5,125 Dante word-locus profiles, 14,306 search documents, 119,579 indexed tokens, 79 authority authors, 17 personaggi, and 296,069 preserved commentary-source rows. These are interface/runtime units, not counts of distinct commentaries or independent scholarly opinions.

## Public Repository And Private Production Boundary

This repository is the **public, citable project entrance** for AF. It is intentionally not a mirror of the private production and research repository used to build and operate the live environment.

The public repository contains material appropriate for inspection, citation, and responsible reuse, including:

- the public website shell under [`demo/frontend`](demo/frontend), without the full runtime data payload;
- selected public static pages, styles, assets, client-side modules, and generators;
- selected method-facing build utilities;
- public runtime checks and deployment-packaging code;
- documentation about the interface, data lineage, rights boundary, and maintenance;
- synthetic or redacted runtime samples under [`sample_runtime`](sample_runtime);
- [`CITATION.cff`](CITATION.cff), [`.zenodo.json`](.zenodo.json), [`LICENSE`](LICENSE), [`LICENSES.md`](LICENSES.md), and [`RELEASE_NOTES.md`](RELEASE_NOTES.md).

The private production repository may additionally contain active development, source-sensitive inputs, internal research material, review traces, generated runtime assets, release coordination, operational state, publication drafts, and other material that does not belong in the public scholarly object.

The two repositories are **not expected to have identical file trees, Git histories, or commit sequences**. A feature may exist on the live AF site without every internal implementation or working artifact being published here.

See [`docs/public/current-status.md`](docs/public/current-status.md) and [`docs/public/public-repository-boundary.md`](docs/public/public-repository-boundary.md) for the current publication boundary.

## GitHub And Zenodo Publication Boundaries

The Zenodo 1.0.0 archive is a narrower, fixed snapshot of the public project. It excludes the full DDP-derived commentary payload and also excludes generated author/work/personaggio pages that may cumulatively expose source-derived material. Both GitHub and Zenodo exclude private research files, publication drafts, reports, snapshots, caches, deployment residue, secrets, credentials, environment files, and source material whose public redistribution has not been established.

The presence of a generated interface page in this repository does not place its source-derived content under the MIT or CC BY licences. See the rights notices below before reusing anything beyond project-owned code or documentation.

## Source And Rights Boundary

DDP is the visible source archive for the commentary layer. Antica Fiamma has written authorisation for the current academic, non-profit website use of DDP-derived material. That authorisation is limited to the authorised website use and is not represented as a licence to redistribute the complete commentary corpus through GitHub, Zenodo, or another repository.

Accordingly, public releases archive project-owned software, documentation, selected method code, public checks, and rights-safe samples rather than the complete live commentary payload. Project-derived scholarly structures are documented and exposed only where their public release does not silently expand rights in underlying source material.

See [`LICENSES.md`](LICENSES.md) and [`docs/public/rights-and-permissions.md`](docs/public/rights-and-permissions.md) for the detailed boundary.

## Repository Guide

- [`docs/public/current-status.md`](docs/public/current-status.md): current relationship between the living public repository, the private production workspace, and the archived 1.0.0 release.
- [`docs/public/repository-guide.md`](docs/public/repository-guide.md): how to read the repository.
- [`docs/public/interface-layers.md`](docs/public/interface-layers.md): scholarly reading layers.
- [`docs/public/data-boundary.md`](docs/public/data-boundary.md): included and excluded data.
- [`docs/public/rights-and-permissions.md`](docs/public/rights-and-permissions.md): rights and permission scope.
- [`docs/public/technical-overview.md`](docs/public/technical-overview.md): implementation overview.
- [`docs/public/sustainability-and-maintenance.md`](docs/public/sustainability-and-maintenance.md): current author-maintained infrastructure.
- [`demo/runtime_checks/README.md`](demo/runtime_checks/README.md): public shell checks.
- [`sample_runtime/README.md`](sample_runtime/README.md): rights-safe structural samples.

## Local Preview

```bash
python3 demo/server.py
```

Then open `http://127.0.0.1:8777/`. The local shell cannot reproduce the complete live site without the separately maintained runtime layer.

## Citation

Use the citation generated from [`CITATION.cff`](CITATION.cff) or the version DOI [`10.5281/zenodo.21479971`](https://doi.org/10.5281/zenodo.21479971). Use [Ruoci Song's ORCID](https://orcid.org/0009-0004-1263-2192) where an author identifier is required. Cite the live environment separately with an access date when referring to its current interface or runtime content.
