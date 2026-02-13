# Project 16: Behavior Cloning vs RL

## Goal
Compare imitation and reinforcement learning with a rigorous protocol that exposes distribution-shift failure modes.

## Implementation Requirements

### Data + BC Pipeline
- [ ] Collect/curate demonstration trajectories with documented expert source.
- [ ] Implement trajectory normalization and train/val/test splitting by episode.
- [ ] Train behavior-cloning policy with early stopping and validation tracking.

### RL Baseline
- [ ] Train an RL baseline on the same task with matched observation/action interfaces.
- [ ] Use equivalent evaluation protocol and metrics across BC and RL.

### Shift Analysis
- [ ] Design at least 3 shifted scenarios (initial-state, dynamics, or observation shift).
- [ ] Quantify BC degradation under shift and compare against RL behavior.

## Validation Gates
- [ ] BC shows strong in-distribution performance with reported confidence intervals.
- [ ] Distribution-shift failures are reproducible and quantified.
- [ ] Comparison includes both sample efficiency and final task success.

## Required Artifacts
- [ ] `docs/bc-vs-rl.md` with dataset protocol and fairness controls.
- [ ] Metrics table for ID vs OOD performance.
- [ ] Example trajectories highlighting failure patterns.
