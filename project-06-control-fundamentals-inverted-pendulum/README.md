# Project 06: Control Fundamentals - Inverted Pendulum

## Goal
Establish strong closed-loop control fundamentals that transfer directly into robotics RL policy design and debugging.

## Implementation Requirements

### System + Controllers
- [ ] Implement nonlinear pendulum dynamics with configurable actuator limits.
- [ ] Derive linearized model around upright equilibrium.
- [ ] Implement PID with anti-windup and derivative filtering.
- [ ] Implement LQR from the linearized state-space model.

### Evaluation Harness
- [ ] Define standard test set: multiple initial angles, impulse disturbances, and sensor noise levels.
- [ ] Record rise time, settling time, overshoot, control effort, and failure count.
- [ ] Use identical evaluation protocol for PID and LQR.

### Robustness Checks
- [ ] Evaluate with actuator saturation enabled.
- [ ] Evaluate with model mismatch (mass/length perturbations).

## Validation Gates
- [ ] Both controllers stabilize from at least +/-15 deg initial offset under nominal dynamics.
- [ ] Disturbance rejection metrics are reported and reproducible.
- [ ] Controller comparison includes at least 3 seeds and summarized uncertainty.

## Required Artifacts
- [ ] `docs/inverted-pendulum-control.md` with controller equations and tuning logic.
- [ ] Reproducible experiment config(s) and plotting script.
- [ ] Comparison table for PID vs LQR performance.
