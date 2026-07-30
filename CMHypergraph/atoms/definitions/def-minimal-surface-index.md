---
id: d064e5a56d03
type: definition
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §2]]"
  - "the index bound for min-max: Marques–Neves, and §4 of the earlier Colding–De Lellis notes"
---

# Definition — index of a minimal surface

How many independent ways a minimal surface can be pushed to lower its
area: the count of unstable directions — a finite integer measuring
instability.

## Statement

> [!definition] Index
> Let $\Sigma \subset M$ be a closed [[def-immersion|immersed]] [[def-minimal-surface|minimal]] surface with [[def-jacobi-operator|Jacobi operator]] $L_\Sigma$. The *index* of $\Sigma$ is the number of negative eigenvalues of $L_\Sigma$, counted with multiplicity. Here $\eta$ is an [[def-eigenvalue|eigenfunction]] with eigenvalue $\lambda$ if $L_\Sigma \eta + \lambda \eta = 0$.

## Notes

> [!note]- Notes (click to expand)
> - A negative eigenvalue of $L_\Sigma$ is a direction along which area decreases to second order (by [[def-jacobi-operator]]); so the index counts independent area-lowering deformations. Index $0$ means *stable* — a local minimum of area.
> - Finiteness is because $\Sigma$ is closed: $L_\Sigma$ is elliptic self-adjoint with discrete spectrum bounded below, so only finitely many eigenvalues are negative.
> - Why *index at most one* in [[prop-minmax-minimal-spheres]]: a one-parameter min-max (a sweepout) produces critical points of index $\le 1$ — the mountain-pass principle. The single unstable direction is the sweep itself.
