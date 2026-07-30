---
id: a8869d7fe33d
type: remark
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, the paragraph following Theorem 1.1]]"
---

# Remark — Where the width inequality's constants come from

An accounting of the three constants in the extinction estimate: two
of them are load-bearing mathematics, one is a bookkeeping artifact —
and knowing which is which is knowing why the argument works.

## Statement

> [!remark] Where the [[def-sweepout-width|width]] inequality's constants come from
> In the width inequality of [[thm-width-evolution]],
> $$
> \frac{d}{dt} W \;\le\; -4\pi \;+\; \frac{3}{4\,(t + C)}\, W,
> $$
> the three constants have three different standings:
>
> - the $4\pi$ is the total curvature of the sphere from [[thm-gauss-bonnet]], entering through [[lem-minimal-sphere-area-decay]] — it is topological, so it cannot degrade as the flow shrinks the manifold;
> - the $\tfrac{3}{4}$ descends from the $\tfrac{3}{2}$ of the scalar-curvature bound [[lem-scalar-curvature-lower-bound]] after multiplication by $\operatorname{Area}/2$ — it is analytic, and its size matters: any coefficient below $1$ makes the correction integrate to a power rather than a logarithm, so it cannot rescue $W$;
> - the $C$ depends only on the initial metric, and its value is irrelevant — it survives surgery because surgery regions carry large positive scalar curvature and never reset the minimum.

## Notes

> [!note]- Notes (click to expand)
> - Both load-bearing constants must hold *exactly*: weaken $4\pi$ to any positive rate and extinction still follows, but lose the topological origin and the rate could degrade with the geometry; raise $\tfrac34$ past $1$ and the integration in [[lem-width-inequality-forces-extinction]] fails.
> - This is the paper's own accounting, promoted from prose to an addressable card.
