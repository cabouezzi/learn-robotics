# Project 10: PPO From Scratch

## Goal
Implement PPO robustly enough for robotics control tasks, including stability diagnostics and reproducible benchmarking.

## Implementation Requirements

### Algorithm Requirements
- [ ] Implement clipped policy objective.
- [ ] Implement value-function loss and entropy bonus.
- [ ] Implement GAE with configurable lambda and gamma.
- [ ] Implement advantage normalization and minibatch SGD epochs.
- [ ] Implement gradient clipping and learning-rate scheduling.

### Training Stability Requirements
- [ ] Log policy KL, entropy, value loss, and explained variance.
- [ ] Add early-stop or warning on excessive KL divergence.
- [ ] Add NaN/inf detection and safe run termination.

### Benchmarking
- [ ] Evaluate on at least one discrete and one continuous task.
- [ ] Run at least 5 seeds per task.
- [ ] Compare against a known baseline implementation (e.g., SB3) under matched settings.

## Validation Gates
- [ ] PPO implementation reaches task success criteria on both benchmark tasks.
- [ ] Variance across seeds is reported, not hidden.
- [ ] At least one unstable run is diagnosed with root-cause analysis and mitigation.

## Required Artifacts
- [ ] `docs/ppo-implementation.md` with equations and pseudocode mapping.
- [ ] Multi-seed result plots and aggregate metrics.
- [ ] Troubleshooting notes for instability cases.
