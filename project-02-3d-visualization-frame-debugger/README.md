# Project 02: 3D Visualization + Frame Debugger

## Goal
Build a frame-debugging tool that makes transform mistakes obvious before they contaminate RL/control experiments.

## Implementation Requirements

### Visualizer Features
- [ ] Render world frame, robot frames, and chained transforms in 3D.
- [ ] Load frame graphs from a config file (`json`/`yaml`).
- [ ] Toggle frame visibility and parent-child relationships interactively.
- [ ] Animate pose interpolation using SLERP for orientation.

### Debug Utilities
- [ ] Show numeric pose readout (`x,y,z` + quaternion or Euler).
- [ ] Add a mode to compare `A->B` vs `B->A` inverse consistency.
- [ ] Add explicit degree/radian conversion UI or CLI checks.

### Tests
- [ ] Test SLERP endpoint correctness and interpolation monotonicity.
- [ ] Test transform-chain order against known reference chains.

## Validation Gates
- [ ] Reproduce at least 5 canonical frame bugs and show correct diagnosis.
- [ ] Visualization confirms expected orientation for right-hand-rule test cases.
- [ ] Inverse/compose checks numerically pass within tolerance (`1e-6` for transform reconstruction).

## Required Artifacts
- [ ] `docs/frame-debugger.md` with usage and bug examples.
- [ ] Screenshots or short clips for each debug scenario.
- [ ] Config examples for at least 2 frame chains.
