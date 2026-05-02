# Lorentz Transformations — Interactive Simulations

Browser-runnable HTML/JavaScript simulations for the openphysica.org course
*Special Relativity & Lorentz Transformations*.

No build step, no dependencies. Just open any `.html` file directly in a
modern browser (Chrome / Firefox / Safari).

## Contents

| File | Topic | Course day |
|---|---|---|
| [`index.html`](index.html) | Landing page with links to all simulations | — |
| [`01-minkowski-diagram.html`](01-minkowski-diagram.html) | Minkowski (x, ct) diagram with two frames; click to place events; Lorentz transformation reported live | Day 2 / Day 6 |
| [`02-two-light-flashes.html`](02-two-light-flashes.html) | Spacecraft flashes light forward and backward simultaneously; demonstrates relativity of simultaneity | Day 5 |
| [`03-time-dilation.html`](03-time-dilation.html) | Light clock comparing proper time and lab time; photon bouncing between mirrors at speed c | Day 3 |
| [`04-length-contraction.html`](04-length-contraction.html) | Proper-length 1m ruler vs. its measurement in a frame where it moves at v | Day 4 |
| [`05-velocity-addition.html`](05-velocity-addition.html) | Plot of relativistic vs Galilean velocity addition; demonstrates that c is a hard upper limit | Day 5 |

## Conventions used in the simulations

- Units where **c = 1** throughout. Time is measured in units of `L/c`, distance in units of `L`.
- Metric signature **(−, +, +, +)** for the spacetime interval: `ds² = −c²dt² + dx² + dy² + dz²`.
- Lorentz factor: `γ = 1 / √(1 − v²/c²)`.
- Forward Lorentz boost from frame S to frame S&prime; (S&prime; moving at +v in S):
  ```
  ct′ = γ (ct − (v/c) x)
  x′  = γ (x  − v t)
  ```

## How to extend

Each simulation is a single self-contained `.html` file with embedded JavaScript
and CSS. To add a new simulation:

1. Copy one of the existing files as a template.
2. Edit the title, explanation, controls, and `draw()` function.
3. Add a row to this README and a card to `index.html`.

## License

Released into the public domain (CC0). Free to copy, modify, and use in any
educational context.
