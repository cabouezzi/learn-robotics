# Project 01: Rigid-Body Geometry Toolkit (Transforms)

## Goal
Implement numerically robust `SO(3)`/`SE(3)` math primitives used later for kinematics, control, and model-based RL.

## Implementation Requirements

### Core Library
- [ ] Implement `hat`, `vee`, `exp_so3`, `log_so3`.
- [ ] Implement quaternion operations: normalize, multiply, inverse, quat <-> rot matrix.
- [ ] Implement `SE(3)` compose/inverse and homogeneous transforms.
- [ ] Implement adjoint transform for twists/wrenches.
- [ ] Support batched operations for vectorized usage.

### Numerical Robustness
- [ ] Handle small-angle regimes with stable approximations.
- [ ] Guard against non-unit quaternions and re-normalize safely.
- [ ] Reject invalid rotations or project to nearest valid rotation when documented.

### Tests
- [ ] Property tests for group closure, inverse consistency, and associativity tolerance.
- [ ] Round-trip tests for quat <-> rot and exp/log maps.
- [ ] Randomized stress tests near singular/edge cases.

## Validation Gates
- [ ] Rotation orthogonality error `||R^T R - I||_F < 1e-6` on random samples.
- [ ] Determinant checks satisfy `|det(R) - 1| < 1e-6`.
- [ ] `exp(log(R))` reconstruction angular error < `1e-5` rad (excluding exact singular cases).

## Required Artifacts
- [ ] API reference in `docs/transforms.md`.
- [ ] `tests/` suite with deterministic seed.
- [ ] Small demo script visualizing compose/inverse correctness.
