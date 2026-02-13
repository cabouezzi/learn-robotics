# Project 05: Contact + Friction Sensitivity Lab

## Goal
Characterize contact/friction behavior and failure modes that commonly destabilize robotic RL training.

## Implementation Requirements

### Simulation Setup
- [ ] Build a tabletop contact scene with at least one push/slide task.
- [ ] Expose friction, restitution, and contact-softness parameters via config.
- [ ] Implement deterministic reset logic with seed control.

### Experiment Design
- [ ] Run a parameter sweep over at least 5 friction settings and 3 contact settings.
- [ ] Execute at least 10 trials per parameter set with fixed seed list.
- [ ] Log slip distance, contact impulse, penetration depth, and settle time.

### Analysis
- [ ] Identify regions with unstable or non-intuitive behavior.
- [ ] Document which contact settings are reliable enough for RL training.

## Validation Gates
- [ ] Sweep is fully reproducible from a single command.
- [ ] Results include summary statistics (mean/std) per parameter set.
- [ ] At least one discontinuity/stiffness-driven failure case is reproduced and explained.

## Required Artifacts
- [ ] `configs/contact_sweep.yaml` (or equivalent).
- [ ] `docs/contact-study.md` with plots/heatmaps.
- [ ] Raw trial logs and a script that regenerates all figures.
