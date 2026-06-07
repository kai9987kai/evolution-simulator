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

## TODO

- Implemented the upgraded web simulator in `Webbots-alpha.html`.
- Added a deterministic seeded PRNG, `window.advanceTime(ms)`, and `window.render_game_to_text()`.
- Added research and model documentation to `README.md`.
- Add deterministic browser hooks and test the major controls.
