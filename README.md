# Evolution Lab

An interactive, research-informed individual-based evolution simulator. Open
`Webbots-alpha.html` in a modern browser; it has no runtime dependencies.

## What evolves

Each organism inherits quantitative traits for speed, body size, sensing,
metabolic efficiency, aggression, sociality, behavioral plasticity, thermal
preference, fecundity, exploration, and lineage colour. Nearby, energy-rich
organisms can reproduce. Their offspring receive recombined parental traits
plus bounded mutations.

There is no fixed fitness score. Survival and reproduction emerge from:

- renewable but locally limited resources;
- energetic costs for movement, body size, sensing, and thermal mismatch;
- a spatial temperature gradient and selectable seasonal or warming regimes;
- behavioral thermoregulation that can buffer thermal mismatch at a cost;
- local competition, mating, predation, ageing, and drought disturbance.

The dashboard tracks population, births, deaths, generation depth, resource
availability, trait diversity, approximate functional ecotypes, mean thermal
lag, and mean plasticity. A drought assay records resistance at the population
nadir and time to recover to 90% of the pre-drought baseline. Click an organism
to inspect its genome. Experiments are reproducible from a text seed.

## Controls

- `Space`: pause or resume
- `F`: toggle fullscreen
- Environment: stable gradient, strong seasons, or rapid warming
- Mutation strength and resource renewal can be changed while running
- Trigger drought applies an 18-second resource-growth shock
- Gene-flow pulse introduces ten warm-adapted migrants from a hypothetical
  source population
- Reset experiment reruns the current seed and settings

## Research basis

The model is exploratory rather than predictive. Its mechanisms were selected
to reflect active research directions:

- Individual variation in energy-budget parameters can scale into population
  dynamics: [Ecological Modelling (2024)](https://doi.org/10.1016/j.ecolmodel.2024.110848)
- Spatially heterogeneous selection can maintain population structure and local
  adaptation: [BMC Ecology and Evolution (2024)](https://doi.org/10.1186/s12862-024-02304-4)
- Mutation can reduce finite-population artefacts in spatial agent-based
  evolutionary models: [Communications Physics (2025)](https://doi.org/10.1038/s42005-025-02120-2)
- Evolution can shift ecological resilience thresholds under stress:
  [Nature Ecology & Evolution (2024)](https://doi.org/10.1038/s41559-024-02543-0)
- Behavioral plasticity can improve persistence while changing the rate of
  inherited adaptation:
  [Nature Communications (2026)](https://doi.org/10.1038/s41467-026-70632-8)
- Populations can appear to adapt while falling progressively behind a moving
  environmental optimum:
  [Scientific Reports (2025)](https://doi.org/10.1038/s41598-025-24445-2)
- Climate-associated gene flow can increase survival under warmer, drier
  conditions, although effects are system-specific:
  [Communications Biology (2025)](https://doi.org/10.1038/s42003-025-08410-3)

The simulator translates these ideas into transparent hypotheses, not fitted
biological parameters. A gene-flow pulse is therefore an intervention to test,
not a guaranteed rescue, and extinction is retained as an outcome rather than
being silently repopulated.

## Earlier experiments

`Base model.py`, `beta.py`, and `3d-version-beta-in-blenderscript` are retained
as historical Turtle and Blender prototypes.
