# ManualDiff

> Semantic revision reports for non-confidential technical manuals.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

ManualDiff is a proposed specialist software tool for Open-hardware maintainers, independent technical writers, and equipment-documentation teams. PDF and Markdown comparisons frequently miss section movement, changed specifications, and consequences for component lists. The intended differentiation is: Traceable section-level text and table comparisons designed for technical revisions.

## Intended users and use cases

- Identify a changed torque specification in a fictional manual
- Detect a renamed section without showing it as deleted
- Compare synthetic Markdown and PDF-derived text outputs

## Planned features

- Extract Markdown and text-layer PDF section structures
- Match similar headings and detect moved, added, or removed sections
- Compare structured parameter tables with unit normalization
- Link changed claims to their source page or heading
- Generate Markdown/HTML evidence reports and structured JSON

## Proposed technology

Python 3.12+, PyMuPDF, markdown-it-py, Typer, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- Markdown and PDF text extractors
- Section segmentation and matching
- Parameter-table differ
- Provenance-aware report output

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Self-authored sample manuals and tables with deliberately edited revisions.`

## Data boundaries and exclusions

OCR of scanned proprietary manuals, distributing third-party copyrighted files, or processing confidential client documentation. All public examples should use Self-authored sample manuals and tables with deliberately edited revisions.

## Known limitations / validation risks

PDF extraction order is unreliable in some layouts; report ambiguities instead of inventing matches.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Professional technical publishing integrations and automated release pipelines. 

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

