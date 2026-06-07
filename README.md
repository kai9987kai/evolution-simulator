# Evolution Lab

An interactive, research-informed individual-based evolution simulator. Open
`Webbots-alpha.html` in a modern browser; it has no runtime dependencies.

## What evolves

Each organism inherits quantitative traits for speed, body size, sensing,
metabolic efficiency, aggression, sociality, thermal preference, fecundity,
exploration, and lineage colour. Nearby, energy-rich organisms can reproduce.
Their offspring receive recombined parental traits plus bounded mutations.

There is no fixed fitness score. Survival and reproduction emerge from:

- renewable but locally limited resources;
- energetic costs for movement, body size, sensing, and thermal mismatch;
- a spatial temperature gradient and selectable seasonal or warming regimes;
- local competition, mating, predation, ageing, and drought disturbance.

The dashboard tracks population, births, deaths, generation depth, resource
availability, trait diversity, and approximate functional ecotypes. Click an
organism to inspect its genome. Experiments are reproducible from a text seed.

## Controls

- `Space`: pause or resume
- `F`: toggle fullscreen
- Environment: stable gradient, strong seasons, or rapid warming
- Mutation strength and resource renewal can be changed while running
- Trigger drought applies an 18-second resource-growth shock
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

## Earlier experiments

`Base model.py`, `beta.py`, and `3d-version-beta-in-blenderscript` are retained
as historical Turtle and Blender prototypes.
