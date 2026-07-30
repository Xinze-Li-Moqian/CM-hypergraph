---
id: c8a7f7c6cfa3
type: theorem
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §4]]"
  - "after Parker–Wolfson bubble trees"
---

# Theorem — Bubble convergence implies varifold convergence

The bridge from the analysts' convergence to the geometers': a sequence
of maps that bubble-converges to a collection of harmonic spheres also
converges to them as varifolds — so the curvature integrals the flow
argument needs pass to the limit.

## Statement

> [!theorem] Bubble convergence implies varifold convergence
> Let $v^j : S^2 \to M$ be $W^{1,2}$ maps [[def-bubble-convergence|bubble-converging]] to a collection $\{u_0, \dots, u_m\}$ of harmonic maps (in the sense of [[def-bubble-convergence]]). Then the associated $2$-[[def-varifold|varifolds]] converge: $V_{v^j} \to \sum_i V_{u_i}$ in the varifold weak-$*$ topology.

## Proof

> [!note]- Proof (click to expand)
> Let $V^j, U_i : S^2 \to G_2 M$ be the Gauss lifts (point plus tangent plane) of $v^j$ and $u_i$, and $J$ the area Jacobian, so the associated [[def-varifold|varifolds]] pair against $h \in C^0(G_2 M)$ as $\int h\circ V^j\, J_{v^j}$.
> 1. **Split the domain by scales.** By (B1)–(B4) choose pairwise-disjoint domains $\Omega^j_0, \dots, \Omega^j_m \subset S^2$ such that $D_{i,j}^{-1}(\Omega^j_i) \to S^2 \setminus \mathcal{S}_i$ and the complement carries no energy in the limit:
> $$
> \lim_{j\to\infty} \int_{S^2 \setminus \cup_i \Omega^j_i} |\nabla v^j|^2 = 0 . \tag{no loss}
> $$
> This uses (B4) — the no-energy-loss clause of [[def-bubble-convergence]] — decisively: the necks joining body to bubbles carry vanishing area.
> 2. **Match each piece to its bubble.** Since area is dominated by energy, the (no loss) bound reduces the claim to showing, for each $i$ and every $h \in C^0(G_2 M)$,
> $$
> \int_{S^2} h\circ U_i\, J_{u_i} \;=\; \lim_{j\to\infty} \int_{\Omega^j_i} h\circ V^j\, J_{v^j} \;=\; \lim_{j\to\infty} \int_{D_{i,j}^{-1}(\Omega^j_i)} h\circ (V^j\circ D_{i,j})\, J_{v^j\circ D_{i,j}} ,
> $$
> the last equality being the change-of-variables formula (the integrand is conformally natural). On $D_{i,j}^{-1}(\Omega^j_i) \to S^2\setminus\mathcal{S}_i$ the rescaled maps converge strongly in $W^{1,2}$ (B1/B2), so the Jacobians and Gauss lifts converge and the limit is $\int h\circ U_i\, J_{u_i}$.
> 3. **Sum.** Adding over $i$ and using (no loss) for the discarded region gives $\int h\circ V^j J_{v^j} \to \sum_i \int h\circ U_i J_{u_i}$ for every $h$ — varifold convergence. $\square$
## Notes

> [!note]- Notes (click to expand)
> - This is CM's Proposition $l{:}bubvar$ (§4). Bubble convergence is a pointwise/energy notion from harmonic-map analysis; varifold convergence is the measure-theoretic notion the [[lem-varifold-quadratic-form|quadratic-form transfer]] and the width evolution consume. The content is that no area is lost in the necks joining body to bubbles.
> - The proof is a strong-convergence-plus-change-of-variables argument; its one real input is (B4) no energy loss, built into [[def-bubble-convergence]]. The deeper fact — that almost-harmonic sequences *do* bubble-converge with no loss — is §5's compactness, a separate layer.
