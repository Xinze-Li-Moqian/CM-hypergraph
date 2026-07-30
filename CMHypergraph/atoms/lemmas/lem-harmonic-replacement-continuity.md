---
id: e8367752e68f
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3]]"
---

# Lemma — Harmonic replacement is continuous

A construction lemma of the tightening (§3), stated here so the
energy-decreasing map's proof cites in-graph nodes, not source labels.

## Statement

> [!lemma] Continuity of harmonic replacement
> The [[def-harmonic-replacement|harmonic replacement]] map $(u, \mathcal{B}) \mapsto H(u, \mathcal{B})$ is continuous from $C^0 \cap W^{1,2}(S^2, M)$ (with balls of small [[def-dirichlet-energy|energy]]) to $C^0 \cap W^{1,2}$: if $u_k \to u$ in $C^0\cap W^{1,2}$ then $H(u_k, \mathcal{B}) \to H(u, \mathcal{B})$.


## Proof

> [!note]- Proof (click to expand)
> Fix a ball collection $\mathcal{B}$ of small energy. On each ball $B \in \mathcal{B}$, $H(u,\mathcal{B})|_B$ is the energy-minimizer with boundary values $u|_{\partial B}$; outside, $H(u,\mathcal{B}) = u$. So continuity reduces to: the small-energy energy-minimizer depends continuously on its boundary values.
> Suppose $u_k \to u$ in $C^0 \cap W^{1,2}$, and let $v_k = H(u_k,\mathcal{B})|_B$, $v = H(u,\mathcal{B})|_B$. Below the [[thm-sacks-uhlenbeck|Sacks–Uhlenbeck]] threshold the minimizer is *unique*, and the map "boundary values $\mapsto$ minimizer" is stable: $v_k$ minimizes energy for boundary data converging to $u|_{\partial B}$, so $E(v_k) \to E(v)$ (the energy is continuous in the boundary data, by comparison with the harmonic extension of $u_k|_{\partial B}$), and the $v_k$ are uniformly small-energy harmonic, hence uniformly smooth by $\epsilon$-regularity ([[lem-epsilon-regularity-harmonic]]). A uniformly-bounded sequence of harmonic maps with converging boundary values and converging energy converges (subsequentially, then fully by uniqueness) in $C^0 \cap W^{1,2}$ to the minimizer $v$ for the limit boundary values. Hence $H(u_k,\mathcal{B}) \to H(u,\mathcal{B})$. $\square$
## Notes

> [!note]- Notes (click to expand)
> - CM Lemma `l:approx` (§3): continuity of the small-energy energy-minimizer on its boundary values (uniqueness from [[thm-sacks-uhlenbeck]] plus stability), needed to patch per-slice replacements into a continuous family in [[thm-energy-decreasing-map]].
> - Proof debt: §3 of the long paper.
