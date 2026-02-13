# Project 18: Learn a Dynamics Model

## Goal
Train a predictive dynamics model suitable for downstream model-based planning.

## Implementation Requirements

### Modeling Pipeline
- [ ] Build dataset of `(state, action, next_state)` tuples from rollouts.
- [ ] Implement normalization and trajectory-aware train/val/test splits.
- [ ] Train a neural dynamics model (single model or ensemble).
- [ ] Support one-step and multi-step rollout evaluation.

### Uncertainty + Robustness
- [ ] If using ensemble/dropout, expose predictive uncertainty estimates.
- [ ] Measure error as rollout horizon increases (1, 5, 10, 20 steps minimum).
- [ ] Analyze where model error is highest in state-action space.

### Engineering Quality
- [ ] Add deterministic training seeds and checkpointing.
- [ ] Log training/validation curves and overfitting diagnostics.

## Validation Gates
- [ ] One-step prediction error is reported on held-out data.
- [ ] Multi-step error accumulation curves are produced and interpreted.
- [ ] Error hotspots are documented with likely causes.

## Required Artifacts
- [ ] `docs/dynamics-modeling.md` with model architecture and training protocol.
- [ ] One-step and multi-step error plots.
- [ ] Analysis of model limits and implications for planning.
