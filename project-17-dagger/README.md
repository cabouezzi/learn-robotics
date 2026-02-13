# Project 17: DAgger

## Goal
Implement iterative dataset aggregation to reduce compounding errors in imitation-based control.

## Implementation Requirements

### DAgger Loop
- [ ] Implement rollout of current policy in target environment.
- [ ] Implement expert query interface for corrective labels.
- [ ] Aggregate new labeled states into dataset with versioned snapshots.
- [ ] Retrain policy after each aggregation round.
- [ ] Run at least 5 DAgger iterations.

### Data + Experiment Control
- [ ] Track number of expert queries per iteration.
- [ ] Track dataset size growth and class/action distribution changes.
- [ ] Keep evaluation protocol fixed across iterations.

### Failure Analysis
- [ ] Identify states where policy repeatedly diverges from expert.
- [ ] Document whether failures are due to perception, control, or coverage gaps.

## Validation Gates
- [ ] Policy performance improves over initial BC baseline across iterations.
- [ ] Compounding-error indicators (e.g., rollout drift) decrease over iterations.
- [ ] Expert labeling budget and performance gains are reported together.

## Required Artifacts
- [ ] `docs/dagger.md` with loop design and expert interface.
- [ ] Iteration-by-iteration performance dashboard/table.
- [ ] Dataset growth report and error analysis notes.
