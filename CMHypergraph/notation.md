---
type: notation
---
# Notation

Every symbol used in a Statement or Proof of this pool, with its defining card. A "debt" entry is notation in use whose definition card does not exist yet — each should eventually graduate into `atoms/definitions/`.

## The cast — role letters

Recurring roles have fixed letters, pool-wide. Graduation translates a
source's lettering into this cast exactly as it translates terminology;
a card's Notes may record the source's original letters.

| Letter | Role |
|---|---|
| $M$, $(M, g)$ | the manifold under study — and the target of every map: $u : S^2 \to M$, $f : \Sigma \to M$ |
| $\Sigma$ | a surface: the domain of a map, a minimal surface, a slice |
| $N$ | a distinguished region or submanifold of $M$ (neck, tube, cap), or the domain of a generic map between manifolds — never the target |
| $u$, $f$ | maps into $M$ |
| $\gamma$ | a sweepout $\gamma^j$ and its slices $\gamma_s$; also a geodesic |
| $[\beta]$ | a homotopy class of sweepouts |
| $g(t)$ | an evolving metric — the flow |
| $E$, $W$ | energy; width ($W^{1,p}$ with a superscript is always the Sobolev space) |
| $X$ | a bare topological space, in purely topological statements |

## The table — notation with its defining card

| Notation | Meaning | Card |
|---|---|---|
| closed manifold | $M$ compact $\wedge\ \partial M = \emptyset$ | [[def-closed-manifold]] |
| simply connected | $X$ path-connected $\wedge\ \pi_1(X) = 1$ | [[def-simply-connected]] |
| $M \cong N$ (manifolds) | $\exists\, \varphi : M \to N$ smooth bijection with $\varphi^{-1}$ smooth | [[def-diffeomorphism]] |
| $G \cong H$ (groups) | group isomorphism | [[def-diffeomorphism]] |
| $M_1 \,\#\, M_2$ | connected sum | [[def-connected-sum]] |
| $\pi_1(X)$ | loops at the basepoint modulo homotopy | [[def-fundamental-group]] |
| $G * H$, $G *_{K} H$ | free product; amalgamated over $K$ | [[def-free-product]] |
| spherical space form $S^3/\Gamma$ | $\Gamma < \mathrm{Isom}(S^3)$ finite $\wedge$ acting freely; the canonical name — never "manifold of constant positive curvature" | [[def-spherical-space-form]] |
| $S^2$-bundle over $S^1$ | the trivial $S^2 \times S^1$ or $\widetilde{S^2 \times S^1}$ | [[def-s2-bundle-over-s1]] |
| $\widetilde{S^2 \times S^1}$ | the unique non-orientable $S^2$-bundle over $S^1$ | [[def-s2-bundle-over-s1]] |
| $\mathbb{R}P^3 \smallsetminus \overline{B^3}$ | punctured $\mathbb{R}P^3$ (open; $\cong \mathbb{R}P^3 \smallsetminus \{pt\}$) — the canonical form | — |
| Ricci flow $\partial_t g = -2\operatorname{Ric}(g)$ | the heat equation for metrics | [[def-ricci-flow]] |
| space-time $({\mathcal M}, \mathbf{t}, \chi, G)$ | time function, time field, horizontal metric | [[def-spacetime]] |
| $({\mathcal M}, G)$ | generalized Ricci flow (space-time with metric) | [[def-generalized-ricci-flow]] |
| $M_t$ | the time-$t$ slice of a space-time | [[def-spacetime]] |
| singular time | a time that is not regular for the flow | [[def-singular-time]] |
| surgery time | synonym: a singular time of a Ricci flow with surgery | [[def-singular-time]] |
| locally separating | two-sided: trivial normal bundle | [[def-locally-separating]] |
| embedded | image of an embedding | [[def-embedding]] |
| $\operatorname{Rm}$ | curvature tensor | [[def-curvature-tensor]] |
| $\operatorname{Ric}$ | Ricci curvature | [[def-ricci-curvature]] |
| $R$ | scalar curvature | [[def-scalar-curvature]] |
| $\nabla$ (connection) | Levi-Civita connection | [[def-levi-civita-connection]] |
| $\triangle = \operatorname{tr}_g \nabla^2$ (on tensors) | rough Laplacian | [[def-rough-laplacian]] |
| $Q(\operatorname{Rm})$ | the quadratic curvature term of the evolution equations | [[thm-curvature-evolution]] |
| $\operatorname{tr}$, $\operatorname{tr}_g$ | trace; $g$-trace | [[def-trace]] |
| $d(x, y)$ | Riemannian distance | [[def-riemannian-distance]] |
| $B(x, r)$ | metric ball $\{ d(x, \cdot) < r \}$ | [[def-riemannian-distance]] |
| $\operatorname{diam}$ | diameter | [[def-diameter]] |
| $\operatorname{Vol}$ | Riemannian volume | [[def-volume]] |
| $\nabla f$ | gradient | [[def-gradient]] |
| $\triangle$ | Laplacian, $\operatorname{div} \circ \operatorname{grad}$ | [[def-laplacian]] |
| $r_y$ | curvature radius: $\sup_{B(y,r_y)} R = r_y^{-2}$ | [[def-curvature-radius]] |
| $\epsilon$-close ($C^{\lfloor 1/\epsilon \rfloor}$) | one dial for accuracy and derivative count | [[def-epsilon-close]] |
| $\epsilon$-neck, central $2$-sphere | rescaled $\epsilon$-approximation of the round cylinder | [[def-epsilon-neck]] |
| $(C,\epsilon)$-cap, core | ball or punctured $\mathbb{R}P^3$ ending in a neck, $C$-controlled | [[def-c-epsilon-cap]] |
| $\epsilon$-tube (open / capped / doubly capped) | union of necks $\cong S^2 \times I$, possibly closed off by caps | [[def-epsilon-tube]], [[def-capped-epsilon-tube]] |
| $\epsilon$-fibration | $S^2$-fibered over $S^1$, a union of necks | [[def-epsilon-fibration]] |
| chain of $\epsilon$-necks (finite / infinite) | necks overlapping in quarter windows, no wrap-around | [[def-neck-chain]] |
| balanced chain | chain stepping one neck-length per car | [[def-balanced-chain]] |
| surgery assumptions | the axioms a Ricci flow with surgery satisfies | debt |
| pinching function; $\Phi$-almost nonnegative curvature | $K \ge -\Phi(R)$, $\Phi(s)/s \to 0$ | [[def-phi-almost-nonnegative-curvature]] |
| $\kappa$-noncollapsed (at scales below $\rho$) | volume $\ge \kappa r^3$ at the curvature scale | [[def-kappa-noncollapsed]] |
| ancient solution | infinite past, complete, non-flat, bounded nonnegative curvature | [[def-ancient-solution]] |
| $\kappa$-solution | an ancient solution, $\kappa$-noncollapsed at all scales | [[def-kappa-solution]] |
| pointed smooth convergence (manifolds / flows) | exhaustion-and-embedding convergence in $C^\infty$ | [[def-pointed-smooth-convergence]] |
| $\Omega_\rho$, thick part | the low-curvature part of the continuing region | [[thm-singular-slice-structure]] |
| curvature evolution; reaction ODE | $\partial_t \operatorname{Rm} = \triangle \operatorname{Rm} + Q$ | [[thm-curvature-evolution]] |
| $\epsilon$-horn (double) | tube whose curvature blows up along an end (both ends) | [[def-epsilon-horn]] |
| $\delta$-neck | an $\epsilon$-neck with the finer parameter $\delta$ | [[def-epsilon-neck]] |
| $\Omega$, continuing region | the bounded-curvature set of a singular slice | [[thm-singular-slice-structure]] |
| $h(t)$, surgery scale | the uniform curvature-radius scale of the surgery necks | [[thm-horn-contains-surgery-neck]] |
| closed canonical component ($C$-component / $\epsilon$-round) | a component that *is* a canonical piece — a space form | [[def-closed-canonical-component]] |
| standard initial metric; standard solution | the capped half-cylinder and its flow — the model glued in at surgery | [[def-standard-solution]], [[thm-standard-solution]] |
| ${\mathcal W}(g, f, \tau)$, $\mu(g, \tau)$ | the entropy and its invariant at scale $\tau$ | [[def-w-entropy]] |
| parabolic rescaling $\hat g = Q\, g(t_0 + Q^{-1} t)$ | the microscope: space by $Q^{1/2}$, time by $Q$ | [[def-parabolic-rescaling]] |
| maximal flow, maximal time | the flow every flow from $g_0$ restricts to | [[def-maximal-flow]] |
| immersion | $df$ injective; image smooth, may self-cross | [[def-immersion]] |
| $A$, second fundamental form | $A(X,Y) = \langle \nabla_X Y, \mathbf n\rangle$; principal curvatures | [[def-second-fundamental-form]] |
| $H$, mean curvature | $\operatorname{tr} A$; the gradient of area | [[def-mean-curvature]] |
| $\lvert A\rvert^2$ | sum of squared principal curvatures | [[def-second-fundamental-form-norm]] |
| branched immersion; branch point, order $b_i$ | immersion off finitely many vanishing-differential points | [[def-branched-immersion]] |
| minimal surface; branched minimal immersion | $H \equiv 0$; the min-max spheres | [[def-minimal-surface]] |
| $E(u)$ | Dirichlet energy of a map $S^2 \to M$ | [[def-dirichlet-energy]] |
| min-max value $k$ of a family | $\inf_H \max_A \mathcal{F}$ over a pinned compact family class | [[def-minmax-value]] |
| mountain-pass value; Palais–Smale condition | the one-parameter min-max; compactness of a functional | [[def-mountain-pass]], [[def-palais-smale]] |
| $W^{1,p}(\Sigma, M)$; $W^{1,2}$ (= $L^2_1$) | Sobolev space of maps, via isometric embedding of the target | [[def-sobolev-space]] |
| $L^p$; weak derivative | integrability classes and derivatives against test functions | [[def-lp-space]], [[def-weak-derivative]] |
| sweepout, $W(g, [\beta])$ | family of $2$-spheres point-to-point; its min-max energy | [[def-sweepout-width]] |
| Jacobi operator $L_\Sigma$; index | second variation of area; count of negative eigenvalues | [[def-jacobi-operator]], [[def-minimal-surface-index]] |
| varifold; varifold distance | surface as mass-with-direction; its weak-$*$ closeness | [[def-varifold]] |
| $M^n_\kappa$, $S_\kappa$ | the constant-curvature model space / surface | [[def-model-space]] |
| Gromov–Hausdorff convergence (pointed) | distance-only convergence; limits may leave manifolds | [[def-gromov-hausdorff-convergence]] |
| Alexandrov space (curvature $\ge k$) | Toponogov comparison read as an axiom | [[def-alexandrov-space]] |
| asymptotic cone $C_\infty X$ | the blow-down limit of a nonnegatively curved space | [[thm-asymptotic-cone]] |
| Toponogov comparison | lower curvature bound makes triangles fat | [[thm-toponogov-comparison]] |
| geodesic (minimizing) | $\nabla_{\gamma'} \gamma' = 0$; length = distance | [[def-geodesic]] |
| prime decomposition; prime | unique factorization under connected sum | [[thm-prime-decomposition]] |
| aspherical | $\pi_n = 0$ for $n \ge 2$; contractible universal cover | [[def-aspherical]] |
| orientable; orientation | an atlas whose coordinate changes preserve it | [[def-orientable]] |
| sphere theorem; free-product subgroup theorem; Hurewicz theorem | the classical inputs, now carded | [[thm-sphere-theorem]], [[thm-free-product-subgroups]], [[thm-hurewicz]] |
| gradient shrinking soliton; $\operatorname{Hess} f$ | $\operatorname{Ric} + \operatorname{Hess} f = g/2\tau$ | [[def-gradient-shrinking-soliton]] |
| ${\mathcal L}$-length, reduced length $l$, reduced volume $\widetilde V$ | the backward-time comparison geometry | [[def-l-length]], [[def-reduced-volume]] |
| curvature operator | the symmetric operator on $\Lambda^2$ induced by $\operatorname{Rm}$ | debt |
| injectivity radius; Busemann function | comparison-chapter terms | debt |
| soul | the compact totally convex core of an open nonnegatively curved manifold | [[thm-soul]] |
| normalized (metric) | $\lvert\operatorname{Rm}\rvert \le 1$ and unit balls at least half-Euclidean | [[def-normalized-initial-metric]] |
| sectional curvature $K(\sigma)$ | the curvature of a tangent $2$-plane | [[def-sectional-curvature]] |
| controlled (flow) | pinched + canonical neighborhoods at scales $\mathbf{r}$ + $\mathbf{K}$-noncollapsed | [[def-controlled-flow]] |
| evolving $\epsilon$-neck (backward time $t'$) | a neck that has been a shrinking cylinder for a while | [[def-evolving-neck]] |
| $(C,\epsilon)$-canonical neighborhood (strong) | neck / cap around the point / closed canonical component | [[def-canonical-neighborhood]] |
| canonical neighborhood assumption | condition 2 of a controlled flow | [[def-controlled-flow]] |
| Ricci flow with surgery | surgery space-time with the flow equation | [[def-ricci-flow-with-surgery]] |
| surgery space-time | space-time whose slices change by surgery at singular times | [[def-surgery-spacetime]] |
| smooth / exposed / singular point | the point trichotomy of a surgery space-time | [[def-smooth-point]], [[def-exposed-point]], [[def-singular-point]] |
| exposed region | the set of exposed points — the newly-added part of a singular slice | [[def-exposed-point]] |
| $G(t)$, horizontal metric | slice-wise metric of a surgery space-time | [[def-ricci-flow-with-surgery]] |

## Ground notions

Primitives the pool takes for granted — deliberately not carded. Anything mathematical that is *not* on this list and *not* in the table above is an undeclared debt.

smooth manifold, smooth map, boundary $\partial M$, compactness, path-connectedness, loop and homotopy, group, quotient, $n$-ball $B^n$ and sphere $S^n$, isometry group
$\mathrm{Isom}$, Riemannian metric, group homomorphism, kernel, normal subgroup, finite group, cyclic group (infinite cyclic $\cong \mathbb{Z}$), connectedness, real projective space $\mathbb{R}P^n$, hyperbolic space $\mathbb{H}^n$, covering map, universal cover, deck group, properly discontinuous action, normal bundle (and its triviality), tubular neighborhood, end of an open manifold, divergence, orthonormal basis, Lie bracket $[X,Y]$, higher homotopy groups $\pi_n$, Euler characteristic $\chi$, singular homology $H_n$, free group, line (a doubly infinite minimizing geodesic), length space, metric cone, integral curve of a vector field, Lie derivative ${\mathcal L}_X$, pullback $\psi^*$ of a tensor by a smooth map, the extension of a connection to tensor fields and its iterates $\nabla^j$, piecewise-smooth curve, the comparison principle for Dini derivatives, Lebesgue measure and measurable functions, test functions $C^\infty_c$.
