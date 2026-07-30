---
id: f4c4f358e240
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §7, Lemma `l:abe`]]"
  - "after Ahlfors–Bers"
---

# Lemma — The conformal parametrization depends continuously on the metric

Uniformization with control: every $C^1$ metric on the sphere has a
unique normalized conformal diffeomorphism to the round one, and it
varies continuously — uniformly Hölder — as the metric varies, as long
as the metrics stay uniformly non-degenerate.

## Statement

> [!lemma] Continuity of the uniformizing map
> Given a $C^1$ metric $\tilde g$ on $S^2$, there is a unique orientation-preserving $C^{1,1/2}$ [[def-conformal-map|conformal diffeomorphism]] $h_{\tilde g} : (S^2, g_0) \to (S^2, \tilde g)$ fixing $3$ given points. Moreover, if $\tilde g_1, \tilde g_2$ are $C^1$ metrics with $\tilde g_i \ge \epsilon\, g_0$, then
> $$
> \|h_{\tilde g_1} - h_{\tilde g_2}\|_{C^0 \cap W^{1,2}} \;\le\; C\, \|\tilde g_1 - \tilde g_2\|_{C^1} ,
> $$
> with $C$ depending on $\epsilon$.


## Proof

> [!note]- Proof (click to expand)
> Existence and uniqueness of the normalized conformal diffeomorphism $h_{\tilde g}$ is the [[thm-measurable-riemann-mapping|measurable Riemann mapping theorem]] applied to the Beltrami coefficient of $\tilde g$ (its conformal structure), normalized by fixing three points. The continuous dependence: if $\tilde g_1, \tilde g_2 \ge \epsilon g_0$, their [[def-beltrami-quasiconformal|Beltrami coefficients]] $\mu_1, \mu_2$ satisfy $\|\mu_1 - \mu_2\|_\infty \le C(\epsilon)\|\tilde g_1 - \tilde g_2\|_{C^1}$ (uniform ellipticity keeps $\|\mu_i\|_\infty$ bounded away from $1$), and the parametric dependence of the solution of the Beltrami equation gives $\|h_{\tilde g_1} - h_{\tilde g_2}\|_{C^0\cap W^{1,2}} \le C\|\mu_1 - \mu_2\|_\infty \le C\|\tilde g_1 - \tilde g_2\|_{C^1}$ — the Lipschitz-in-the-coefficient clause of [[thm-measurable-riemann-mapping]]. $\square$
## Notes

> [!note]- Notes (click to expand)
> - This is CM's Lemma `l:abe` (§7), after Ahlfors–Bers. Existence and uniqueness of the normalized uniformizing map is [[thm-measurable-riemann-mapping|classical]]; the content is the *continuous dependence* on the metric, which is what lets a family of area-minimizing parametrizations be assembled into a continuous sweepout.
> - Proof debt: the Ahlfors–Bers theory of the Beltrami equation with parameters; $C^{1,1/2}$ regularity and the Lipschitz dependence on the (uniformly elliptic) metric.
