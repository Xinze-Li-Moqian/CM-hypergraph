---
id: 10faaddbdc22
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Appendix A, (A.7)–(A.9)]]"
  - "the balancing is the original device introduced by Hersch (following that method)"
---

# Lemma — Hersch balancing

Any conformal parametrization of the sphere can be recentered so that
its coordinate functions have no first-eigenfunction component — a
fixed-point argument that makes the test functions admissible.

## Statement

> [!lemma] Hersch balancing
> Let $\Sigma$ be a topological $2$-sphere, $\eta > 0$ a positive function on $\Sigma$ with $\int_\Sigma \eta > 0$, and $\Phi : \Sigma \to S^2 \subset \mathbb{R}^3$ a [[def-conformal-map|conformal diffeomorphism]]. Then there is a conformal automorphism $\psi$ of $S^2$ such that the coordinate functions $\phi_i = x_i \circ (\psi \circ \Phi)$ satisfy
> $$
> \int_\Sigma \eta\, \phi_i \;=\; 0 \qquad (i = 1, 2, 3) .
> $$


## Proof

> [!note]- Proof (click to expand)
> The [[def-conformal-map|conformal]] automorphisms of $S^2$ are parametrized by the open unit ball $B^3$: for $a \in B^3$, let $\psi_a$ be the Möbius map fixing $\pm a/|a|$ and moving mass toward $a$ (as $|a| \to 1$, $\psi_a$ concentrates near $a/|a|$). Define $\mathcal{A} : B^3 \to \mathbb{R}^3$ by the $\eta$-weighted center of mass of the pushed coordinates,
> $$
> \mathcal{A}(a) = \frac{\int_\Sigma \eta\, (x \circ (\psi_a \circ \Phi))}{\int_\Sigma \eta} \in \mathbb{R}^3 ,
> $$
> continuous on $B^3$. As $a \to a_0 \in \partial B^3 = S^2$, the map $\psi_a\circ\Phi$ concentrates all mass at $a_0$, so $\mathcal{A}(a) \to a_0$: $\mathcal{A}$ extends continuously to the boundary as the identity $S^2 \to S^2$. A continuous map $\overline{B^3} \to \overline{B^3}$ restricting to the identity (degree $1$) on the boundary is surjective — in particular $0$ is in its image (else $\mathcal{A}: \overline{B^3}\to \overline{B^3}\setminus\{0\}$ would retract to $\partial B^3$ as the identity, contradicting Brouwer / $\pi_2(S^2) \neq 0$). So there is $a$ with $\mathcal{A}(a) = 0$: setting $\psi = \psi_a$, the coordinates $\phi_i = x_i \circ(\psi\circ\Phi)$ satisfy $\int_\Sigma \eta\,\phi_i = 0$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - The mechanism (the proof debt): the conformal automorphisms of $S^2$ are parametrized by the open unit ball $B_1(0) \subset \mathbb{R}^3$ (their "centers of mass"); the map sending a center to the $\eta$-weighted center of mass of the pushed coordinates extends continuously to the identity on the boundary $\partial B_1$, so by a Brouwer-degree / topological argument it has a zero — the balanced $\psi$. This is CM's (A.7)–(A.9).
> - This balancing, following Hersch's original method, is the device that lets the coordinate functions serve as test functions in [[lem-second-eigenvalue-test]]: the single constraint $\int \eta\phi_i = 0$ is met for all three coordinates at once.
