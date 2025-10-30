# ROADMAP — wcct-umatrix

**Milestone:** v0.2  |  **Board:** wcct-umatrix v0.2
- Milestone: https://github.com/QCT-xyz/wcct-umatrix/milestone/1
- Project board: https://github.com/orgs/QCT-xyz/projects/1

## Goals (v0.2)
1) Prereg multi-seed CI  (Issue #1)
   - Add CI job that runs 3 seeds on a tiny grid and aggregates Spearman, MI, Jaccard, enrichment.
   - Artifacts: publish/robustness_multi_seed.json, plot image in publish/.
   - Acceptance: CI passes; summary keys present; seeds ≥ 3; thresholds documented in PR.
   - Link: https://github.com/QCT-xyz/wcct-umatrix/issues/1

2) Watershed baseline vs U-ridges  (Issue #2)
   - Implement watershed on |∇φ|; compute Jaccard and enrichment vs U-ridge map.
   - Add a simple ROC under circular-shift null.
   - Artifacts: publish/watershed_comparison.png, publish/watershed_metrics.csv.
   - Acceptance: notebook cell(s) + figure + CSV; brief comparison note committed.
   - Link: https://github.com/QCT-xyz/wcct-umatrix/issues/2

3) 3D stack check  (Issue #3)
   - Stack slices to form a 3D U volume; extract ridge surfaces; compare overlap with 3D high-|∇φ| tubes.
   - Artifacts: publish/stack3d_overlap.png, short JSON with overlap stats.
   - Acceptance: figure + JSON; brief methods note; baseline comparison stated.
   - Link: https://github.com/QCT-xyz/wcct-umatrix/issues/3

## Targets & ownership
- Target window: next 30 days
- Owner: Dustin Thornton (QCT)

## Share pack (stable links)
- Colab: https://colab.research.google.com/github/QCT-xyz/wcct-umatrix/blob/main/env/U_matrix_WCCT.ipynb
- Release v0.1: https://github.com/QCT-xyz/wcct-umatrix/releases/tag/v0.1

## Notes
- Keep research code and notebook here; keep deploy/infra in wcct-harness.
- CI should stay fast: favor tiny grids and NumPy-only paths in GitHub Actions.
