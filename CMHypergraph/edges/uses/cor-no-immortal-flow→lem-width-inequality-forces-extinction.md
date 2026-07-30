---
id: ec5e96e6561c
kind: uses
ref:
  - "[[cor-no-immortal-flow]]"
  - "[[lem-width-inequality-forces-extinction]]"
---

# `cor-no-immortal-flow` → `lem-width-inequality-forces-extinction`

**uses**: [[cor-no-immortal-flow]] uses [[lem-width-inequality-forces-extinction]] — the proof consumes the target.

**instantiation**:
- $W(t) := W(g(t), [\beta])$ — the [[def-sweepout-width|width]] of the smooth flow along the fixed class, supplied with its inequality by [[thm-width-evolution]];
- $C :=$ the constant of [[lem-scalar-curvature-lower-bound]] for $g(0)$;
- hypothesis check: $W \ge 0$ by definition of the width; continuous in $t$ since the energies of a fixed sweepout vary smoothly with the metric; defined on all of $[0, \infty)$ by the immortality assumption.
