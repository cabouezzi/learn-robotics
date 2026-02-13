# Project 14: Robustness + Domain Randomization

## Goal
Demonstrate sim-to-real style robustness gains using domain randomization and stress testing.

## Implementation Requirements

### Training Variants
- [ ] Train baseline policy without randomization.
- [ ] Train randomized policy with documented randomization ranges.
- [ ] Keep algorithm, architecture, and training budget matched between variants.

### Randomization Dimensions
- [ ] Randomize mass/inertia within physically plausible ranges.
- [ ] Randomize sensor noise models.
- [ ] Randomize action delay/latency.
- [ ] Optionally randomize friction/contact parameters if relevant.

### Stress-Test Matrix
- [ ] Build an out-of-distribution evaluation matrix covering each perturbation type.
- [ ] Evaluate both policies on identical perturbation seeds and scenarios.

## Validation Gates
- [ ] Randomized policy outperforms baseline on OOD matrix in majority of scenarios.
- [ ] In-domain performance drop (if any) is quantified and explained.
- [ ] Safety violations/terminations are tracked and compared.

## Required Artifacts
- [ ] `docs/domain-randomization.md` with training/eval protocol.
- [ ] OOD robustness tables and plots.
- [ ] A concise recommendation on deploy-time randomization strategy.
