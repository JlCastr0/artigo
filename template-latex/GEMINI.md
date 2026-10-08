# Academic Project Context: SBC LaTeX Template (TCC)

## Project Overview
This repository contains the LaTeX source code and bibliography for the academic research paper/TCC:
- **Title**: *Avaliação de Modelos de Linguagem de Grande Escala na Geração Dinâmica de Diálogos para Personagens Não Jogáveis em Jogos de Investigação*
- **Format**: SBC (Sociedade Brasileira de Computação) LaTeX template.
- **Language**: Portuguese (with English Abstract).

## Main Project Files
- `sbc-template.tex`: Main document source file.
- `sbc-template.bib`: BibTeX bibliography database.
- `sbc-template.sty`, `sbc.bst`, `caption2.sty`: SBC formatting and bibliography style definitions.
- `assets/`: Image and figure assets.

## Academic Writing Agents & Skills (Workspace-Scoped)
This workspace is equipped with the local **Academic Writing multi-agent suite**, installed exclusively under `.gemini/`:

### Orchestrator Skill
- **`academic`** (defined in `.gemini/skills/academic/SKILL.md`): Orchestrates reviews, research, drafting, polishing, and audits.
- **Canonical Principles**: `.gemini/skills/academic/references/academic-writing.md` (30 codified principles across Structure, Prose, Math, Figures, Citations, and Process).

### Specialized Subagents (`.gemini/agents/`)
- **Review (Read-only)**:
  - `@consistency-checker`: Terminology, cross-references, figure-text alignment, structural coherence.
  - `@logic-reviewer`: Argument flow, narrative arc, transitions, logical gaps.
  - `@technical-reviewer`: Methodological soundness, mathematical rigor, technical claims.
  - `@writing-reviewer`: Academic tone, clarity, conciseness, grammar.
  - `@latex-layout-auditor`: Float placement, PDF layout checks, alignment.
- **Audit**:
  - `@bibliography-auditor`: BibTeX completeness, arXiv normalization, venue consistency.
- **Research & Ideation**:
  - `@research-analyst`: Related work, gap analysis, research positioning.
  - `@brainstormer`: Alternative framings, conceptual connections, novel angles.
  - `@paper-crawler`: API querying (DBLP + OpenAlex) for literature surveys.
- **Action (Editing/Writing)**:
  - `@prose-polisher`: Surgical rewrites improving clarity and conciseness while preserving author intent.
  - `@section-drafter`: Drafting sections, transitions, captions, and abstracts following SBC standards.
  - `@latex-figure-specialist`: TikZ/pgfplots figures and float formatting.

## Build and Compilation Workflow
To compile the document to PDF:
```bash
pdflatex -interaction=nonstopmode sbc-template.tex
bibtex sbc-template
pdflatex -interaction=nonstopmode sbc-template.tex
pdflatex -interaction=nonstopmode sbc-template.tex
```
