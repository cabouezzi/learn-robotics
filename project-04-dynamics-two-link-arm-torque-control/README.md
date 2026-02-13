# Project 04: Dynamics of a Two-Link Arm (Torque Control)

## Goal
Build and validate a dynamics simulator that exposes integration stability issues relevant to RL training.

## Implementation Requirements

### Dynamics Model
- [ ] Derive equations of motion for a 2-link planar arm (Lagrangian form).
- [ ] Implement forward dynamics `qdd = f(q, qd, tau)`.
- [ ] Include gravity, Coriolis/centrifugal, and mass-matrix terms.
- [ ] Add actuator saturation limits.

### Integrators + Stability Study
- [ ] Implement explicit Euler and semi-implicit Euler.
- [ ] Make timestep configurable and sweep multiple values.
- [ ] Reproduce exploding simulation behavior under unstable settings.
- [ ] Stabilize with integration/timestep/damping adjustments.

### Instrumentation
- [ ] Log joint states, control torques, total energy, and constraint violations.
- [ ] Plot energy drift over rollout horizons.

## Validation Gates
- [ ] Unstable configuration is reproducibly demonstrable.
- [ ] Stable configuration runs for full horizon without numeric blow-up.
- [ ] In low-damping/no-control mode, energy trend is physically plausible and documented.

## Required Artifacts
- [ ] `docs/dynamics.md` with equations and implementation notes.
- [ ] Plots comparing integrators and timesteps.
- [ ] Reproduction script for unstable vs stabilized runs.
