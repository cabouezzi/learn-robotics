# Project 12: Manipulation Suite in MuJoCo/Isaac

## Goal
Build a manipulation benchmark suite that reflects real robotics RL engineering work (task design, rewards, resets, and failure analysis).

## Implementation Requirements

### Task Suite
- [ ] Implement one arm+gripper environment with unified observation/action interfaces.
- [ ] Implement Reach task with clear success condition.
- [ ] Implement Push task with clear success condition.
- [ ] Implement Pick-and-place task with clear success condition.

### Training Setup
- [ ] Choose and justify control interface (position, velocity, or torque action space).
- [ ] Implement reward functions with documented shaping terms per task.
- [ ] Implement randomized reset distribution for object/goal starts.
- [ ] Log per-episode success/failure reason codes.

### Iteration Discipline
- [ ] Track reward-shaping revisions with rationale and observed effect.
- [ ] Track observation-space revisions and their effect on stability/performance.
- [ ] Maintain one shared evaluation protocol across all tasks.

## Validation Gates
- [ ] Evaluate each task on at least 100 episodes with fixed seed list.
- [ ] Reach and Push achieve >= 80% success; Pick-and-place achieves >= 60% success (or documented blocker analysis).
- [ ] Failure taxonomy identifies top recurring failure modes and mitigations.

## Required Artifacts
- [ ] `docs/manipulation-suite.md` with task specs and success definitions.
- [ ] Per-task training/eval curves and success-rate tables.
- [ ] Changelog of reward/observation/reset design decisions.
