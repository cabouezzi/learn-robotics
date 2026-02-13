# Project 07: Arm Tracking + Disturbance Rejection

## Goal
Build trajectory tracking that remains stable under realistic disturbance/noise conditions.

## Implementation Requirements

### Tracking Stack
- [ ] Implement time-parameterized joint trajectories (at least sinusoidal and cubic).
- [ ] Implement PD + feedforward controller for joint tracking.
- [ ] Add configurable disturbance injection (torque pulses and external force equivalents).
- [ ] Add configurable sensor noise on joint states.

### Metrics + Analysis
- [ ] Compute per-joint RMSE, max absolute error, and phase lag.
- [ ] Report tracking degradation under each disturbance/noise profile.
- [ ] Implement and evaluate at least one mitigation strategy (retuned gains, filter, or feedforward update).

### Robustness Engineering
- [ ] Enforce joint limits and safe torque limits.
- [ ] Add detector for tracking divergence and fail-safe stop.

## Validation Gates
- [ ] Nominal tracking run meets predefined RMSE target (document threshold per joint).
- [ ] Disturbance/noise runs show measurable degradation relative to nominal.
- [ ] Mitigation reduces error by a documented margin vs disturbed baseline.

## Required Artifacts
- [ ] `docs/tracking-robustness.md` with disturbance protocol and outcomes.
- [ ] Plot set for nominal vs disturbed vs mitigated runs.
- [ ] Reproducible scripts/configs for all experiments.
