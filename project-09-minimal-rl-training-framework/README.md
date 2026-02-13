# Project 09: Minimal RL Training Framework

## Goal
Create a reusable RL experimentation framework suitable for robotics policy research.

## Implementation Requirements

### Framework Architecture
- [ ] Implement modular training pipeline (`agents/`, `envs/`, `train`, `evaluate`).
- [ ] Add config-driven experiments (YAML/TOML/CLI overrides).
- [ ] Add structured logging for returns, episode length, losses, entropy, and timing.
- [ ] Add checkpoint save/resume and model version metadata.

### Reproducibility + Ops
- [ ] Centralize seed handling across env, policy, and replay/storage components.
- [ ] Add run IDs and artifact directories per experiment.
- [ ] Add automatic periodic evaluation during training.

### Baseline Environments
- [ ] Train/evaluate on CartPole.
- [ ] Train/evaluate on at least one continuous-control toy task.

## Validation Gates
- [ ] Re-running same seed reproduces near-identical learning curves (document tolerance).
- [ ] Checkpoint resume reproduces uninterrupted training trend.
- [ ] Framework supports at least 3-seed aggregate reporting.

## Required Artifacts
- [ ] `docs/rl-framework.md` with architecture and run instructions.
- [ ] Example configs for discrete and continuous tasks.
- [ ] Experiment summary table across seeds.
