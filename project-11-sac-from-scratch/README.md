# Project 11: SAC From Scratch

## Goal
Implement SAC with production-level stability controls for continuous robotic control.

## Implementation Requirements

### Algorithm Requirements
- [ ] Implement twin Q-networks and target Q-networks.
- [ ] Implement stochastic squashed-Gaussian policy.
- [ ] Implement entropy-regularized objective with automatic temperature tuning.
- [ ] Implement soft target updates with configurable `tau`.
- [ ] Implement replay buffer with configurable capacity and warmup.

### Stability + Instrumentation
- [ ] Log Q-target statistics, TD error, entropy, alpha, and action distribution stats.
- [ ] Add gradient norm monitoring and NaN guards.
- [ ] Add configurable update-to-data ratio.

### Benchmarking
- [ ] Benchmark on at least 2 continuous-control tasks.
- [ ] Compare to PPO under matched environment and evaluation protocol.
- [ ] Run at least 5 seeds per method/task.

## Validation Gates
- [ ] SAC trains stably without recurrent divergence on benchmark tasks.
- [ ] Sample efficiency comparison (return vs environment steps) is reported.
- [ ] Performance variance across seeds is explicitly documented.

## Required Artifacts
- [ ] `docs/sac-implementation.md` with update equations and design choices.
- [ ] Learning-curve plots for SAC vs PPO.
- [ ] Debug log excerpts from at least one instability investigation.
