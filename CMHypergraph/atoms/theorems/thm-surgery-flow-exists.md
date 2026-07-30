---
id: 0d29e7eb76c3
type: theorem
references:
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, chs. 13–17; the inductive construction is Theorem 15.9]]"
  - "[[thm-15-9]]"
  - "[[ref-kleinerlott|Kleiner & Lott, §II.4–II.5]]"
  - "[[prop-ii-5]]"
  - "[[ref-perelman2|Perelman II, §§4–5]]"
  - "[[ref-caozhu|Cao & Zhu, §7 — the same construction in a third notation]]"
  - "[[ref-bbbmp|Bessières–Besson–Boileau–Maillot–Porti, an independent surgery variant]]"
  - "[[ref-tao-ricci-notes|Tao's lecture notes, a step-by-step analytic walkthrough]]"
  - "[[ref-bamler-surgery|Bamler, Ricci flow with surgery, ch. 7 — a compact self-contained account of the whole construction]]"
---

# Theorem — Existence of the Ricci flow with surgery

## Statement

> [!theorem] Existence of the [[def-ricci-flow-with-surgery|Ricci flow with surgery]]
> Let $(M, g_0)$ be a [[def-closed-manifold|closed]] Riemannian $3$-manifold containing no [[def-embedding|embedded]], [[def-locally-separating|locally separating]] $\mathbb{R}P^2$. Then there is a [[def-ricci-flow-with-surgery|Ricci flow with surgery]] with initial metric $(M, g_0)$ such that:
>
> 1. it is defined for all $t \in [0, \infty)$;
> 2. its [[def-singular-time|surgery times]] form a discrete subset of $[0, \infty)$;
> 3. the topological change across a [[def-singular-time|surgery time]] is a [[def-connected-sum|connected-sum]] decomposition together with removal of components, each [[def-diffeomorphism|diffeomorphic]] to one of
>
> $$
> S^2 \times S^1, \qquad \mathbb{R}P^3 \,\#\, \mathbb{R}P^3, \qquad \widetilde{S^2 \times S^1}, \qquad S^3/\Gamma .
> $$

## Proof

> [!note]- Proof — citation chain (click to expand)
> **Data.** [[thm-controlled-flow-extension]] provides sequences $\mathbf{K} = \{\kappa_i\}$, $\Delta = \{\delta_i\}$, $\mathbf{r} = \{r_i\}$; fix a non-increasing $\bar\delta(t) \le \delta_i$ on $[T_{i-1}, T_i)$, and let $\Phi$ be the pinching function of [[thm-phi-pinching]]. Rescale $g_0$ so that it is [[def-normalized-initial-metric|normalized]] — rescaling reparametrizes the flow and touches no conclusion.
>
> 1. **The maximal smooth flow.** The manifold $M$ is closed, so [[thm-short-time-existence]] applies to $(M, g_0)$ and yields a [[def-maximal-flow|maximal]] smooth Ricci flow
> $$
> g(t), \quad t \in [0, T_0), \qquad g(0) = g_0, \qquad T_0 < \infty \implies \sup_M |{\operatorname{Rm}}(\cdot, t)| \to \infty .
> $$
> If $T_0 = \infty$: a smooth flow is a Ricci flow with surgery with empty surgery set, and conclusions 1–3 hold trivially. Assume $T_0 < \infty$.
> 2. **The smooth flow is controlled**, i.e. satisfies the three conditions of [[def-controlled-flow]] with parameters $(\Phi, \mathbf{r}, \mathbf{K})$ on $[0, T_0)$:
>    - *Condition 1.* $M$ is closed and $g_0$ normalized — the hypotheses of [[thm-phi-pinching]]; its conclusion, every sectional curvature $\ge -\Phi(R)$ at every $(x, t)$, is condition 1 verbatim.
>    - *Condition 3.* Apply [[thm-no-local-collapsing]] with $(T, \rho) := (T_0, \epsilon)$: it returns $\kappa(T_0, \epsilon) > 0$ such that every ball $B(x, r)$, $r < \epsilon$, with $|{\operatorname{Rm}}| \le r^{-2}$ on it satisfies $\operatorname{Vol} B(x, r) \ge \kappa r^3$.
>    - *Condition 2.* Pinching and noncollapsing are exactly the hypotheses of [[thm-canonical-neighborhood]]; applied with $(\epsilon, \kappa, \Phi)$ it returns $r_0 > 0$ such that every point with $R(x, t) \ge r_0^{-2}$ has a strong [[def-canonical-neighborhood|canonical neighborhood]].
>    - Both conditions 2 and 3 weaken as their parameters decrease, and the sequences $\mathbf{r}, \mathbf{K}$ may be assumed to lie below $r_0$ and $\kappa$ on each finite interval; so the flow is controlled with $(\Phi, \mathbf{r}, \mathbf{K})$.
> 3. **Extension to all time.** The flow of steps 1–2 satisfies every hypothesis of [[thm-controlled-flow-extension]]: it is a Ricci flow with surgery on $[0, T_0)$ (no surgeries, so the surgery assumptions hold vacuously), controlled with $(\Phi, \mathbf{r}, \mathbf{K})$. Its conclusion yields a Ricci flow with surgery $({\mathcal M}, G)$ with
> $$
> \mathbf{t}({\mathcal M}) = [0, \infty), \qquad (M_0, G(0)) = (M, g_0),
> $$
> controlled with the same parameters, surgeries performed at the scale set by $\bar\delta$. This is conclusion 1.
> 4. **Discreteness.** Let $S \subset [0, \infty)$ be the set of singular times of ${\mathcal M}$. By [[def-surgery-spacetime]], $S$ is discrete; by [[def-singular-time]], $S$ is exactly the set of surgery times. This is conclusion 2.
> 5. **The topological change.** Fix $T \in S$ and write $M_{T^-}$ for the pre-surgery slice, $M_T$ for the post-surgery slice, and
> $$
> \Omega \;=\; \Big\{ x \in M_{T^-} : \sup_{t < T} R(x, t) < \infty \Big\}
> $$
> for the continuing region.
>    - *(a) Where the cut happens.* The flow satisfies the canonical neighborhood condition at scale $r(T)$ — step 3 — which is the hypothesis of [[thm-singular-slice-structure]]. Its conclusions: $\Omega$ is open with smooth limit metric $\bar g$; every end of $\Omega$ is an $\epsilon$-[[def-epsilon-horn|horn]]; every component of $M_{T^-}$ missing $\Omega$ consists of points with canonical neighborhoods. Apply [[thm-horn-contains-surgery-neck]] with $\delta := \bar\delta(T)$: each horn attached to the thick part contains a $\bar\delta(T)$-[[def-epsilon-neck|neck]] $N_j$ centered at [[def-curvature-radius|curvature radius]] $h(T)$; let $S_j \subset N_j$ be its central sphere, $j = 1, \dots, k$.
>    - *(b) The cut.* The surgery removes the horn ends beyond the $S_j$ and every component missing $\Omega$, and seals each boundary sphere with a copy of the [[def-standard-solution|standard]] cap ($\cong B^3$). Denote by $X_1, \dots, X_m$ the discarded *closed* components.
>    - *(c) Connected-sum recovery.* Each $S_j$ is an [[def-embedding|embedded]] $2$-sphere with trivial normal bundle — its neck $N_j \cong S^2 \times (-1, 1)$ *is* a tubular neighborhood — so [[lem-sphere-surgery]] applies to each in turn: cutting and capping realizes, with $n$ the number of non-separating spheres among the $S_j$,
> $$
> M_{T^-} \;\cong\; M_T \,\#\, X_1 \,\#\, \cdots \,\#\, X_m \,\#\, \big(S^2 \times S^1\big)^{\,\#\, n} .
> $$
> This is the [[def-connected-sum|connected-sum]] decomposition of conclusion 3.
>    - *(d) The discarded list.* Each $X_i$ misses $\Omega$, so by (a) each of its points has a canonical neighborhood. If some point's neighborhood is a [[def-closed-canonical-component|closed canonical component]], then $X_i$ is that component and $X_i \cong S^3/\Gamma$, a [[def-spherical-space-form|spherical space form]]. Otherwise every point of $X_i$ lies in an $\epsilon$-neck or a $(C,\epsilon)$-[[def-c-epsilon-cap|cap]] — the hypothesis of [[prop-manifolds-covered-by-caps-and-necks]] — whose closed cases give
> $$
> X_i \;\cong\; S^3, \quad \mathbb{R}P^3, \quad \mathbb{R}P^3 \,\#\, \mathbb{R}P^3, \quad \text{or an } S^2\text{-bundle over } S^1 .
> $$
> Since $S^3$ and $\mathbb{R}P^3$ are themselves $S^3/\Gamma$, and the $S^2$-[[def-s2-bundle-over-s1|bundles]] over $S^1$ are $S^2 \times S^1$ and $\widetilde{S^2 \times S^1}$, every $X_i$ is on the list of conclusion 3. $\square$

## Notes

> [!note]- Notes (click to expand)
> - **Picture.**
>   ![[surgery.svg|673]]
> - The [[def-locally-separating|locally separating]] hypothesis is vacuous for orientable manifolds (see that card); it bites only in the non-orientable case.
> - **Why exclude it**: a locally separating $\mathbb{R}P^2$ makes quotient necks $\mathbb{R}P^2 \times \mathbb{R}$ possible in the high-curvature region — a legitimate model whose cross-section is not a sphere, so it cannot be closed off by gluing a $3$-ball. Excluding it, every neck the surgery meets is a genuine $S^2$-neck.
> - This is the endpoint of the entire surgery program: canonical neighborhoods at high curvature, surgery on $\delta$-necks, non-accumulation of surgery times. Pool material: [[thm-15-9]] (the technical construction), the morgantian ch-13–17 chapters, [[prop-ii-5]] for the Kleiner–Lott form.
> - The outline above is a pure citation chain: every inference consumes a cited card. The analytic load sits on the cited cards — [[thm-short-time-existence]], [[thm-phi-pinching]], [[thm-no-local-collapsing]] (proved, via the entropy cards), [[thm-canonical-neighborhood]], [[thm-singular-slice-structure]], [[thm-horn-contains-surgery-neck]], and the extension engine [[thm-controlled-flow-extension]]. The standard cap now has its cards: [[def-standard-solution]] and [[thm-standard-solution]].
