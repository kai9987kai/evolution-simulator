Original prompt: innovate imrpove refine and advance look at new and best research to help

## Direction

- Make `Webbots-alpha.html` the primary, dependency-free simulator.
- Replace random, non-heritable neural-network movement with an inspectable individual-based eco-evolutionary model.
- Ground the model in energy-budget tradeoffs, spatially heterogeneous selection, heritable mutation/recombination, and measurable diversity.

## Research translated into the model

- Individual energy budgets and trait variation affect population-level dynamics.
- Spatial and temporal environmental heterogeneity can maintain local adaptation.
- Mutation helps prevent small simulated populations from losing all strategy diversity through finite-size drift.
- Eco-evolutionary feedbacks can move resilience thresholds, so disturbances should alter both ecology and subsequent selection.

- Implemented the upgraded web simulator in `Webbots-alpha.html`.
- Added a deterministic seeded PRNG, `window.advanceTime(ms)`, and `window.render_game_to_text()`.
- Added research and model documentation to `README.md`.
- Reworked perception to periodic cached sensing so population growth does not create a quadratic scan on every physics tick.

## Verification

- JavaScript syntax and `git diff --check` pass.
- The game harness produced canvas screenshots and structured state without console errors.
- A long run reached day 70.7 with 158 living organisms, 490 births, 396 deaths, nine generations, and three functional ecotypes.
- Verified pause/resume, reset, drought, environment selection, speed selection, organism inspection, desktop layout, and the 390px mobile breakpoint.
- Browser console reported no errors.

## TODO

- In progress: replace the non-periodic thermal gradient's wraparound topology with bounded habitat edges.
- In progress: add evolvable behavioral plasticity, climate-lag metrics, disturbance recovery tracking, and a gene-flow experiment.
