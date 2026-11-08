# ManualDiff - technical plan

**Planning document, not an implementation report.**

## Product objective

Traceable section-level text and table comparisons designed for technical revisions.

## Intended system boundary

- **Input:** Self-authored sample manuals and tables with deliberately edited revisions.
- **Processing stages:** Markdown and PDF text extractors; Section segmentation and matching; Parameter-table differ; Provenance-aware report output.
- **Output:** A pair of self-authored manuals yields a correct, source-linked change report.
- **Runtime / build stack (tentative):** Python 3.12+, PyMuPDF, markdown-it-py, Typer, pytest
- **Explicitly excluded:** OCR of scanned proprietary manuals, distributing third-party copyrighted files, or processing confidential client documentation.

## Functional modules

- Extract Markdown and text-layer PDF section structures
- Match similar headings and detect moved, added, or removed sections
- Compare structured parameter tables with unit normalization
- Link changed claims to their source page or heading
- Generate Markdown/HTML evidence reports and structured JSON

## Demonstration and acceptance cases

**Test 1:** Identify a changed torque specification in a fictional manual

**Test 2:** Detect a renamed section without showing it as deleted

**Test 3:** Compare synthetic Markdown and PDF-derived text outputs

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

PDF extraction order is unreliable in some layouts; report ambiguities instead of inventing matches.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
