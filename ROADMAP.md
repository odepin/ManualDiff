# ManualDiff - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A pair of self-authored manuals yields a correct, source-linked change report.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Implement Markdown structure parser | 9 | Heading hierarchy with source spans |
| 2 | Build PDF text and page extraction | 10 | Page-labeled text and layout warnings |
| 3 | Create section similarity matcher | 11 | Moved/changed sections differentiated in fixtures |
| 4 | Add specification table comparison | 10 | Unit-aware sample checks |
| 5 | Generate evidence-rich reports | 8 | Linked source page and section references |
| 6 | Tests and user documentation | 10 | Reference manuals and explicit limitations |
| | **Total estimated** | **58** | |

## Detailed milestones

### 1. Implement Markdown structure parser (9 estimated hours)

- [ ] Deliverable: Heading hierarchy with source spans.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Build PDF text and page extraction (10 estimated hours)

- [ ] Deliverable: Page-labeled text and layout warnings.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Create section similarity matcher (11 estimated hours)

- [ ] Deliverable: Moved/changed sections differentiated in fixtures.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Add specification table comparison (10 estimated hours)

- [ ] Deliverable: Unit-aware sample checks.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Generate evidence-rich reports (8 estimated hours)

- [ ] Deliverable: Linked source page and section references.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Tests and user documentation (10 estimated hours)

- [ ] Deliverable: Reference manuals and explicit limitations.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: PDF extraction order is unreliable in some layouts; report ambiguities instead of inventing matches.
- Commercial hypothesis (not validated): Professional technical publishing integrations and automated release pipelines.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
