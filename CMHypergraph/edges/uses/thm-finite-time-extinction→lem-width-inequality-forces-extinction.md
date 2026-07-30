---
id: 6b4d28981ccd
kind: uses
ref:
  - "[[thm-finite-time-extinction]]"
  - "[[lem-width-inequality-forces-extinction]]"
---

# `thm-finite-time-extinction` → `lem-width-inequality-forces-extinction`

**uses**: [[thm-finite-time-extinction]] uses [[lem-width-inequality-forces-extinction]] — the proof consumes the target.

**instantiation**:
- $W(t) :=$ the component-maximum width function of [[lem-surgery-preserves-width-inequality]] — *not* the width of any single class;
- $C :=$ the constant of [[lem-scalar-curvature-lower-bound]], never reset by surgeries;
- hypothesis check: $W \ge 0$ as a maximum of widths; continuous between surgery times, and the lemma is applied on each smooth interval — the downward jumps at surgery times only strengthen the chained integrated form.
