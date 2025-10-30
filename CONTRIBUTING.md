# Contributing to WCCT × U-Matrix

Thanks for considering a contribution. This repo contains a reproducible notebook and curated publish artifacts.

## How to propose changes
- Open an Issue first (Bug or Feature template) and describe the motivation.
- For code/notebook changes, fork and create a feature branch.
- Keep PRs focused; include a short rationale and screenshots or key metrics if relevant.

## Development checklist
- Notebook runs end-to-end (Cells 0–21) without errors on a clean environment.
- CI passes (smoke + mini-run).
- No large binaries added; keep artifacts in env/wcct_umatrix_outputs/publish/ only.

## Style
- Prefer small, readable cells. Keep prose in Markdown cells.
- Pin deps in requirements.txt; avoid adding heavy extras.

## Security & disclosures
- Do not include secrets or tokens in notebooks or commits.
- If you believe you’ve found a security issue, open a SECURITY.md-guided disclosure (or email the maintainer).
