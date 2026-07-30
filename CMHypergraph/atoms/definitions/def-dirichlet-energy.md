---
id: a7470faae0f7
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 18]]"
---

# Definition — energy of a map

The Dirichlet energy of a map from the sphere: how much total stretching the map does — an upper bound for the area it sweeps, with equality exactly for the conformal maps.

## Statement

> [!definition] Energy of a map from $S^2$
> Let $(M, g)$ be a Riemannian manifold and $u : S^2 \to M$ a smooth map. The *energy* of $u$ is
> $$
> E(u) \;=\; \frac{1}{2} \int_{S^2} |du|^2 \, d\mathrm{vol},
> $$
> where $|du|$ is the norm of the differential computed with the round metric on $S^2$ and with $g$ on $M$, and $d\mathrm{vol}$ is the [[def-volume|volume]] measure of the round metric. The definition extends to maps of Sobolev class $W^{1,2}$.

## Notes

> [!note]- Notes (click to expand)
> - In two dimensions the energy is conformally invariant in the source: replacing the round metric on $S^2$ by any conformal metric leaves $E(u)$ unchanged — so no choice is being made.
> - Always $\operatorname{Area}(u) \le E(u)$, with equality exactly when $u$ is a branched conformal map: energy is area plus the cost of non-conformal parametrization. This is why min-max over energy and over area give the same width.
