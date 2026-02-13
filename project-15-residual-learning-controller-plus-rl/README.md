# Project 15: Residual Learning (Controller + RL)

## Goal
Combine classical control priors with RL residuals to improve robustness and smoothness.

## Implementation Requirements

### Controller Composition
- [ ] Implement base controller (PID/LQR/tracking) with stable standalone behavior.
- [ ] Implement residual policy output that is added to base-controller action.
- [ ] Add residual-action scaling and clipping safeguards.
- [ ] Add switch to compare base-only, RL-only, and residual-hybrid modes.

### Training + Safety
- [ ] Train residual policy with reward terms that discourage fighting base controller.
- [ ] Add penalties or constraints for unsafe/high-frequency residual actions.
- [ ] Log base action, residual action, and combined action separately.

### Evaluation
- [ ] Evaluate all three modes under nominal and disturbed conditions.
- [ ] Measure tracking error, control effort, smoothness (e.g., action jerk proxy), and failure count.

## Validation Gates
- [ ] Residual-hybrid outperforms base-only on at least one robustness metric.
- [ ] Residual-hybrid avoids instability seen in RL-only under matched conditions.
- [ ] Cases where residual harms behavior are documented with mitigation attempts.

## Required Artifacts
- [ ] `docs/residual-rl.md` with architecture and reward design.
- [ ] Comparative plots/tables for base-only vs RL-only vs hybrid.
- [ ] Failure-case notes and revised safeguards.
