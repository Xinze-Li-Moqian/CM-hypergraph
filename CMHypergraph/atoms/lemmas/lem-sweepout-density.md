---
id: 3d36f51cbd08
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §7, Lemma `l:density`]]"
---

# Lemma — Sweepouts can be regularized

Every sweepout is approximable by a smooth one: given a $W^{1,2}$
family of spheres, there is a nearby homotopic family with $C^2$
slices depending continuously in $C^2$ — so both the energy and area
widths may be computed on smooth families.

## Statement

> [!lemma] Density of smooth sweepouts
> Given a [[def-sweepout-width|sweepout]] $\gamma \in \Omega$ and $\epsilon > 0$, there is a regularization $\tilde\gamma$ homotopic to $\gamma$ with
> $$
> \max_t \|\tilde\gamma(\cdot, t) - \gamma(\cdot, t)\|_{W^{1,2}} \le \epsilon ,
> $$
> each slice $\tilde\gamma(\cdot, t)$ is $C^2$, and $t \mapsto \tilde\gamma(\cdot, t)$ is continuous from $[0,1]$ to $C^2(S^2, M)$.


## Proof

> [!note]- Proof (click to expand)
> Mollify in both variables. Fix a smooth mollifier on $S^2$ and on $[0,1]$. Given the sweepout $\gamma \in W^{1,2}$, first reparametrize slightly so the endpoint constant slices are exactly constant on a collar. Convolve $\gamma(\cdot, t)$ with the spatial mollifier at scale $\rho$: each slice becomes $C^\infty$ into $\mathbb{R}^N \supset M$, and (small energy / nearest-point projection to $M$, valid since the mollified map is $W^{1,2}$-close to a map into $M$) project back to $M$ to get $C^2$ slices. Convolve in $t$ at scale $\rho$ to make $t \mapsto \tilde\gamma(\cdot,t)$ continuous into $C^2$. Mollification converges in $W^{1,2}$: $\max_t\|\tilde\gamma(\cdot,t)-\gamma(\cdot,t)\|_{W^{1,2}} \to 0$ as $\rho \to 0$, so choose $\rho$ with the bound $\le \epsilon$. The mollified family is homotopic to $\gamma$ (linear interpolation stays a sweepout for $\rho$ small) and has constant endpoints, hence lies in $\Omega_\gamma$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - This is CM's Lemma `l:density` (§7). Regularizing the family without raising the maximal energy much is what lets the energy width $W_E$ and the area width $W_A$ both be evaluated on smooth families, where the pointwise energy–area comparison applies.
> - Proof debt: mollification of the family in the source variable together with a diagonal argument to keep it a sweepout; standard but with the continuity in $C^2$ requiring care.
