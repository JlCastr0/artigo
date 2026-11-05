# Bibliographic Verification & Audit Plan

## Objective
Audit the 45 entries in `monografia/referencias.bib` using scholarly databases (CrossRef, PubMed, OpenAlex) to identify hallucinatory, incorrect, or mismatched sources, and update the bibliography with correct metadata.

## Key Files & Context
- `monografia/referencias.bib`
- Academic Search Skill (`nature-academic-search`)

## Implementation Steps
1. **Automated Audit:** Invoke the `generalist` sub-agent to parse `referencias.bib` and run continuous queries against academic databases (CrossRef, PubMed, arXiv) for each entry.
2. **Analysis & Report:** The sub-agent will classify each citation as `verified`, `mismatch`, `not_found`, or `suspicious`, producing a detailed audit report.
3. **Review:** Present the audit report and proposed corrections to the user for approval.
4. **Correction:** Apply the approved corrections to `monografia/referencias.bib` (fixing titles, authors, years, or venues).

## Verification & Testing
- Ensure `main.tex` compiles successfully via `pdflatex` and `bibtex` after any modifications to the `.bib` file.
- Verify that every cited source in the final document corresponds to a real, verifiable publication.