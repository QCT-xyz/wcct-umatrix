# WCCT x U-Matrix

[![smoke](https://github.com/QCT-xyz/wcct-umatrix/actions/workflows/smoke.yml/badge.svg)](https://github.com/QCT-xyz/wcct-umatrix/actions/workflows/smoke.yml)
[![mini-run](https://github.com/QCT-xyz/wcct-umatrix/actions/workflows/mini-run.yml/badge.svg)](https://github.com/QCT-xyz/wcct-umatrix/actions/workflows/mini-run.yml)


Reproducible notebook linking WCCT scalar fields to U-Matrix coherence boundaries with falsifiable metrics, null tests, and robustness sweeps.

## One-click (after first push)
Colab:
    https://colab.research.google.com/github/QCT-xyz/wcct-umatrix/blob/main/env/U_matrix_WCCT.ipynb
Binder:
    https://mybinder.org/v2/gh/QCT-xyz/wcct-umatrix/main?labpath=env%2FU_matrix_WCCT.ipynb

## Run locally
    python -m venv .venv
    source .venv/bin/activate
    pip install -r requirements.txt
    jupyter lab
Open env/U_matrix_WCCT.ipynb and run cells 0–21 in order.
Outputs land in env/wcct_umatrix_outputs/publish/.

## Contents
- env/U_matrix_WCCT.ipynb — main notebook
- env/wcct_umatrix_outputs/publish/ — figure composite, figure note, summaries
- requirements.txt — pinned deps
- .gitignore — ignores venv and bulky outputs

## Notes
- Keep research here (wcct-umatrix). Keep Cloud Run/infra in wcct-harness.
- Push via HTTPS; macOS Keychain can store your token for future pushes.
