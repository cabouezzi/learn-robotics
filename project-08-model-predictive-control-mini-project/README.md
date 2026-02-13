# Project 08: Model Predictive Control (MPC) Mini-Project

## Goal
Implement constrained MPC in a way that mirrors model-based decision loops used in robotics autonomy stacks.

## Implementation Requirements

### MPC Core
- [ ] Implement finite-horizon shooting MPC for cart-pole or 2-link arm.
- [ ] Support configurable horizon length, timestep, and cost weights.
- [ ] Enforce actuator and state constraints inside optimization.
- [ ] Implement warm-starting from previous solution.

### Runtime + Reliability
- [ ] Run in receding-horizon loop and log solve time per step.
- [ ] Add fallback behavior when optimization fails (last action, safe action, or backup controller).
- [ ] Add constraint-violation counters.

### Comparative Baseline
- [ ] Compare against a simpler controller (PD/LQR) using identical tasks.

## Validation Gates
- [ ] MPC loop executes at a documented minimum control frequency (define target and measure achieved rate).
- [ ] Constraint violations are rare and explicitly reported.
- [ ] Horizon/cost ablation demonstrates expected performance tradeoffs.

## Required Artifacts
- [ ] `docs/mpc-mini-project.md` with formulation and solver choices.
- [ ] Benchmark results vs baseline controller.
- [ ] Failure-case analysis and mitigation notes.
