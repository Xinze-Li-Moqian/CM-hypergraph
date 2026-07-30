---
id: d0a5c189d062
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §§1–2]]"
  - "[[ref-sacksuhlenbeck|Sacks & Uhlenbeck, §1, Theorem 1.6 — harmonic and weakly conformal implies branched immersion]]"
  - "the branched-immersion notion and the proof of 1.6 are Gulliver–Osserman–Royden"
---

# Definition — branched immersion

An immersion with finitely many bad points: away from them it is a
genuine immersion, at them the differential vanishes to finite order —
the way harmonic maps of the sphere degenerate.

## Statement

> [!definition] Branched immersion
> A smooth map $f : \Sigma \to M$ from a surface is a *branched immersion* if there is a finite set $\{p_1, \dots, p_k\} \subset \Sigma$ — the *branch points* — such that $f$ is an [[def-immersion|immersion]] on $\Sigma \setminus \{p_i\}$, and near each $p_i$, in suitable [[def-conformal-map|conformal]] coordinates $z$ centered at $p_i$, $df$ vanishes exactly to order $b_i \ge 1$ — the *branching order*. A *branched conformal immersion* is one that is angle-preserving where it is an immersion.

## Notes

> [!note]- Notes (click to expand)
> - The local model at a branch point of order $b$ is $z \mapsto z^{b+1}$: the map wraps the disc $b+1$ times, and the image has a cusp-like singularity. Away from the $p_i$ the image is a smooth [[def-immersion|immersed]] surface.
> - Branch points enter through the min-max: the [[prop-minmax-minimal-spheres|minimal spheres realizing the width]] arise as limits of harmonic maps, which may branch. In the [[thm-gauss-bonnet|Gauss–Bonnet]] count each branch point of order $b_i$ contributes $+2\pi b_i$ to the total curvature — the reason branch points *help* the area-decay estimate.
