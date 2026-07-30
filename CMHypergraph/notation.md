---
type: notation
---
# Notation

Every symbol this network uses, with the card that defines it.

The table covers the cards in this repository. It was inherited from a larger
pool and carried forty-four rows for symbols whose defining cards are not
published here; a symbol table that mostly points nowhere is worse than a
shorter one that resolves.

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
| $M \cong N$ (manifolds) | $\exists\, \varphi : M \to N$ smooth bijection with $\varphi^{-1}$ smooth | [[def-diffeomorphism]] |
| $G \cong H$ (groups) | group isomorphism | [[def-diffeomorphism]] |
| $M_1 \,\#\, M_2$ | connected sum | [[def-connected-sum]] |
| $\pi_1(X)$ | loops at the basepoint modulo homotopy | [[def-fundamental-group]] |
| $G * H$, $G *_{K} H$ | free product; amalgamated over $K$ | [[def-free-product]] |
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
| $\operatorname{Vol}$ | Riemannian volume | [[def-volume]] |
| $\nabla f$ | gradient | [[def-gradient]] |
| $\triangle$ | Laplacian, $\operatorname{div} \circ \operatorname{grad}$ | [[def-laplacian]] |
| surgery assumptions | the axioms a Ricci flow with surgery satisfies | debt |
| curvature evolution; reaction ODE | $\partial_t \operatorname{Rm} = \triangle \operatorname{Rm} + Q$ | [[thm-curvature-evolution]] |
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
| aspherical | $\pi_n = 0$ for $n \ge 2$; contractible universal cover | [[def-aspherical]] |
| curvature operator | the symmetric operator on $\Lambda^2$ induced by $\operatorname{Rm}$ | debt |
| injectivity radius; Busemann function | comparison-chapter terms | debt |
| sectional curvature $K(\sigma)$ | the curvature of a tangent $2$-plane | [[def-sectional-curvature]] |
| Ricci flow with surgery | surgery space-time with the flow equation | [[def-ricci-flow-with-surgery]] |
| surgery space-time | space-time whose slices change by surgery at singular times | [[def-surgery-spacetime]] |
| smooth / exposed / singular point | the point trichotomy of a surgery space-time | [[def-smooth-point]], [[def-exposed-point]], [[def-singular-point]] |
| exposed region | the set of exposed points — the newly-added part of a singular slice | [[def-exposed-point]] |
| $G(t)$, horizontal metric | slice-wise metric of a surgery space-time | [[def-ricci-flow-with-surgery]] |

## Ground notions

Primitives the pool takes for granted — deliberately not carded. Anything mathematical that is *not* on this list and *not* in the table above is an undeclared debt.

smooth manifold, smooth map, boundary $\partial M$, compactness, path-connectedness, loop and homotopy, group, quotient, $n$-ball $B^n$ and sphere $S^n$, isometry group
$\mathrm{Isom}$, Riemannian metric, group homomorphism, kernel, normal subgroup, finite group, cyclic group (infinite cyclic $\cong \mathbb{Z}$), connectedness, real projective space $\mathbb{R}P^n$, hyperbolic space $\mathbb{H}^n$, covering map, universal cover, deck group, properly discontinuous action, normal bundle (and its triviality), tubular neighborhood, end of an open manifold, divergence, orthonormal basis, Lie bracket $[X,Y]$, higher homotopy groups $\pi_n$, Euler characteristic $\chi$, singular homology $H_n$, free group, line (a doubly infinite minimizing geodesic), length space, metric cone, integral curve of a vector field, Lie derivative ${\mathcal L}_X$, pullback $\psi^*$ of a tensor by a smooth map, the extension of a connection to tensor fields and its iterates $\nabla^j$, piecewise-smooth curve, the comparison principle for Dini derivatives, Lebesgue measure and measurable functions, test functions $C^\infty_c$.
