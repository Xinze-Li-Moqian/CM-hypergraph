---
id: 1db98f0335fe
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §§1–2]]"
  - "[[ref-sacksuhlenbeck|Sacks & Uhlenbeck, §1, Corollary 1.7 — a harmonic map of the sphere is a conformal branched minimal immersion]]"
  - "[[ref-docarmo|do Carmo, Riemannian Geometry, ch. 6]]"
  - "[[ref-leeriemannian|Lee, Introduction to Riemannian Manifolds, ch. 8]]"
---

# Definition — minimal surface

A surface in equilibrium for area: its mean curvature vanishes everywhere, so no small push lowers the area to first order — the
critical points of the area functional, and the surfaces the min-max
produces.

## Statement

> [!definition] Minimal surface
> An [[def-immersion|immersed]] surface $\Sigma \subset M$ is *minimal* if its [[def-mean-curvature|mean curvature]] vanishes identically, $H \equiv 0$. A *branched minimal immersion* of $S^2$ is a [[def-branched-immersion|branched conformal immersion]] $S^2 \to M$ that is minimal where it is an immersion.

## Notes

> [!note]- Notes (click to expand)
> - Minimal = critical for area, not area-minimizing: $H \equiv 0$ is the Euler–Lagrange equation of the area functional (see [[def-mean-curvature]]), a stationarity condition, and a minimal surface may well be an unstable saddle — which is exactly what min-max produces.
> - The one consequence the flow arguments consume: with $H = \kappa_1 + \kappa_2 = 0$ the principal curvatures are $\pm\lambda$, so $\det A = -\lambda^2 = -\tfrac12 |A|^2$ (see [[def-second-fundamental-form-norm]]). This specializes the [[lem-gauss-equation|Gauss equation]] to $K_\Sigma = K_M - \tfrac12|A|^2$ and drives the minimal-sphere area decay.
> - A conformal harmonic map of $S^2$ *is* a branched minimal immersion — the form in which [[prop-minmax-minimal-spheres]] delivers them. Mechanism (Sacks–Uhlenbeck §1, Corollary 1.7): the Hopf differential of a harmonic map is holomorphic, $S^2$ carries no nontrivial holomorphic quadratic differential, so harmonicity forces weak conformality; then harmonic + weakly conformal is a branched immersion (their Theorem 1.6, after Gulliver–Osserman–Royden), minimal where immersed.
