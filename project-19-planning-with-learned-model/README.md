# Project 19: Planning with a Learned Model

## Goal
Plan actions with a learned dynamics model and compare against model-free RL under equal evaluation constraints.

## Implementation Requirements

### Planner
- [ ] Implement shooting-based planner (CEM/MPPI or equivalent) over learned dynamics.
- [ ] Add configurable horizon, population size, and action constraints.
- [ ] Add uncertainty-aware scoring/penalty if uncertainty estimates are available.
- [ ] Add fallback behavior when planner confidence is low or optimization fails.

### Comparative Protocol
- [ ] Compare against PPO and SAC on the same task and state/action definitions.
- [ ] Use matched evaluation seeds and consistent success metrics.
- [ ] Track sample efficiency as return vs environment interaction count.

### Shift Robustness
- [ ] Evaluate planner and model-free baselines under changed physics.
- [ ] Report failure modes unique to learned-model planning.

## Validation Gates
- [ ] Planning system reaches usable task performance with documented sample budget.
- [ ] Comparative analysis clearly reports where model-based is better/worse.
- [ ] Changed-physics results include quantitative robustness metrics.

## Required Artifacts
- [ ] `docs/model-based-planning.md` with planner details and tuning strategy.
- [ ] Efficiency and robustness comparison plots/tables vs PPO/SAC.
- [ ] Postmortem notes for planner failure cases.
