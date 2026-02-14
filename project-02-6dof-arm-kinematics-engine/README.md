# Project 02: 6-DOF Arm Kinematics Engine

## Timeline
4-6 weeks

## Goal
Implement forward/inverse kinematics and Jacobian-based tooling for a 6-DOF manipulator.

## Build Checklist
- [ ] Load robot from URDF
- [ ] Implement forward kinematics (joint to end-effector pose)
- [ ] Implement geometric Jacobian computation
- [ ] Implement inverse kinematics: pseudoinverse and damped least squares
- [ ] Handle joint limits and singularities
- [ ] Validate against simulator (MuJoCo or PyBullet)

## Deliverable Checklist
- [ ] Kinematics repository with tests
- [ ] Demo video of IK tracking a target

## Starter Structure
- `src/`
- `tests/`
- `docs/`
- `artifacts/`
