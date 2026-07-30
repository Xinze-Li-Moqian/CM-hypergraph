---
id: 57cedabe3da6
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, Theorem in §1, proof §6]]"
---

# Lemma — Harmonic replacement decreases energy definitely

The local engine of the whole construction: replacing a small-energy
map on a disc by the harmonic map with the same boundary lowers the
energy by at least half the energy of the difference.

## Statement

> [!lemma] [[def-harmonic-replacement|Harmonic replacement]] energy gain
> There is $\epsilon_1 > 0$ (depending on $M$) such that if $u, v : B_1 \subset \mathbb{R}^2 \to M$ are $W^{1,2}$ maps agreeing on $\partial B_1$, with $v$ [[def-weakly-harmonic-map|weakly harmonic]] of [[def-dirichlet-energy|energy]] at most $\epsilon_1$, then
> $$
> \int_{B_1} |\nabla u|^2 \;-\; \int_{B_1} |\nabla v|^2 \;\ge\; \tfrac12 \int_{B_1} |\nabla v - \nabla u|^2 .
> $$

## Proof

> [!note]- Proof (click to expand)
> Since $u = v$ on $\partial B_1$, Stokes' theorem gives
> $$
> \int_{B_1}|\nabla u|^2 - \int_{B_1}|\nabla v|^2 - \int_{B_1}|\nabla(u-v)|^2 \;=\; -2\int_{B_1}\langle u - v,\, \triangle v\rangle \;=:\; \Psi ,
> $$
> so it suffices to bound $|\Psi| \le \tfrac12\int|\nabla(u-v)|^2$.
> 1. **The harmonic map equation.** As $v$ is weakly harmonic into $M \subset \mathbb{R}^N$, its tension field $\triangle v$ is normal to $M$, with $|\triangle v| \le |\nabla v|^2 \sup_M |A|$ ($A$ the [[def-second-fundamental-form|second fundamental form]]).
> 2. **Almost-tangency.** For a smooth closed $M$ there is $C$ with $|(x-y)^N| \le C|x-y|^2$ for $x, y \in M$ (either $|x-y| \ge 1/C$ and it is trivial, or $x-y$ is nearly tangent). Applied to $u(x), v(x) \in M$: $|(u-v)^N| \le C|u-v|^2$.
> 3. **Estimate $\Psi$.** Since $\triangle v$ is normal, $\langle u-v, \triangle v\rangle = \langle (u-v)^N, \triangle v\rangle$, so by steps 1–2, $|\Psi| \le 2C\int |u-v|^2\,|\nabla v|^2\sup|A|$.
> 4. **Hardy closes it.** In conformal coordinates the small-energy harmonic $v$ has $|\nabla v|^2 = |\zeta|^2$ up to controlled factors for a holomorphic $\zeta$ (Hélein's Coulomb-gauge regularity); applying the [[lem-hardy-holomorphic|holomorphic Hardy inequality]] with $h = |u-v|$ (which vanishes on $\partial B_1$) bounds $\int|u-v|^2|\nabla v|^2$ by a small multiple of $\int|\nabla(u-v)|^2$. Taking the energy threshold $\epsilon_1$ small enough that this multiple is $\le \tfrac12$ gives $|\Psi| \le \tfrac12\int|\nabla(u-v)|^2$. $\square$
## Notes

> [!note]- Notes (click to expand)
> - This is CM's Theorem $l{:}trivmap$ (§6). It is the quantitative core: harmonic replacement not only lowers energy but does so by a definite fraction of how far the map was from harmonic — which is what makes the tightening [[thm-energy-decreasing-map]] converge and gives the modulus $\Psi$.
> - The proof is now a citation chain: the [[def-tension-field|harmonic map equation]] and almost-tangency (elementary geometry of $M$) reduce the energy difference to a cross term, closed by the [[lem-hardy-holomorphic|holomorphic Hardy inequality]] — itself resting on the [[lem-wente|Wente lemma]]. The one remaining debt is [[thm-helein-regularity|Hélein's regularity theorem]], whose Coulomb-gauge / moving-frame argument puts $|\nabla v|^2$ in the holomorphic form Hardy needs.
