# Project 03: Kinematics of a 6-DOF Arm

## Goal
Implement production-grade kinematics tooling for a 6-DOF manipulator and validate against a physics simulator.

## Implementation Requirements

### Kinematics Stack
- [ ] Parse URDF and build a kinematic tree.
- [ ] Implement forward kinematics for all links and end-effector.
- [ ] Implement analytic or geometric Jacobian for end-effector pose.
- [ ] Implement IK with pseudoinverse and damped least squares.
- [ ] Implement joint-limit handling and explicit solver status codes (`success`, `max_iter`, `infeasible`, `singular`).

### Robustness + Diagnostics
- [ ] Add Jacobian condition-number monitoring.
- [ ] Add damping schedule or fixed damping with documented rationale.
- [ ] Add finite-difference Jacobian checker for regression tests.

### Simulator Cross-Validation
- [ ] Validate FK/Jacobian against MuJoCo or PyBullet for random joint states.
- [ ] Validate IK on random reachable targets sampled from simulator rollouts.

## Validation Gates
- [ ] FK position error vs simulator median < `2e-3 m`.
- [ ] FK orientation error vs simulator median < `1.0 deg`.
- [ ] IK success rate >= `90%` on reachable targets (with limits enforced).
- [ ] Unreachable targets return non-success status without crashing.

## Required Artifacts
- [ ] `docs/kinematics.md` with solver design and failure modes.
- [ ] Benchmark script with reproducible random seeds.
- [ ] Test report with FK/Jacobian/IK metrics.
