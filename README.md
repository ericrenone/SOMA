# SOMA

## *The Triality of Area — One Invariant, Three Tongues*

---

## Abstract

A triangle has an area. So does a polygon. So does a lattice region. The same scalar can be derived from three radically different inputs — edge lengths, vertex coordinates, or counts of integer points — and each derivation is a complete theory unto itself. **SOMA** posits that this is not a coincidence of elementary geometry but a *trilingual signature* of a single underlying invariant, and that the same triality reappears at every level of physics where an area-like quantity governs an observable: phase-space action, Berry curvature flux, entanglement area, and the Hund exchange integral. The framework gives the conversion grammar between these three "tongues" and uses it to unify intrinsic, extrinsic, and topological descriptions of energy.

---

## 1 · The three tongues

Let $T \subset \mathbb{R}^2$ be a simple polygon with vertices $\mathbf{v}_1, \dots, \mathbf{v}_n$.

**Tongue I — Intrinsic (lengths only).** For a triangle with sides $a, b, c$ and semiperimeter $s = (a+b+c)/2$,

$$A = \sqrt{s(s-a)(s-b)(s-c)}$$

This is the *intrinsic* description: the triangle does not need to be embedded anywhere. The data are scalar invariants of the metric. Generalised to any $n$-simplex, this becomes the Cayley–Menger determinant — a single $(n+2)\times(n+2)$ determinant in pairwise squared distances.

**Tongue II — Extrinsic (vertices only).** The shoelace formula

$$A = \tfrac{1}{2}\left|\sum_{i=1}^{n}(x_i\, y_{i+1} - x_{i+1}\, y_i)\right|$$

uses no edge lengths. It uses an embedding into $\mathbb{R}^2$ and a chosen orientation. The interior is never touched: information flows only through the *boundary, traversed once*. This is Stokes' theorem in its discrete clothing.

**Tongue III — Topological (interior & boundary points).** For a *lattice* polygon,

$$A = I + \tfrac{B}{2} - 1$$

where $I$ counts strictly-interior lattice points and $B$ counts boundary points. No metric. No coordinates. Just two integers and a constant. This is *combinatorial topology*: the area is the Euler-characteristic-weighted lattice census.

> **Thought experiment.** Hand three observers a region of the floor. Give the first only a tape measure, the second only chalk to mark corners, the third only a bag of pennies and the rule "place one on every grid intersection inside or on the edge." All three return — independently, by different paths — with the same number. If three blind men can each find an elephant by touching it differently, the elephant is real.

---

## 2 · The Rosetta principle

Define the **SOMA invariant** $\mathcal{S}$ as the equivalence class of all triples $(\text{intrinsic data},\ \text{extrinsic data},\ \text{topological data})$ that compute the same scalar. The three tongues are linked by a triangle of dictionaries:

- **I → II:** *Embedding.* Lengths plus a base point and a heading determine vertices uniquely up to rigid motion. The Cayley–Menger determinant vanishes precisely when the configuration *fails to embed* in the ambient dimension — the algebraic test for realisability.
- **II → III:** *Refinement.* Shrink the lattice spacing to zero and Pick's formula limits to Shoelace. Pick is Shoelace's *integer shadow*; Shoelace is Pick's continuum closure.
- **III → I:** *Coarse-graining.* Given enough lattice points, the boundary census reconstructs the metric up to lattice-scale ambiguity. Distance geometry's central inverse problem.

Each arrow loses information one way and gains it the other. The *closed* triangle of arrows is the algebraic content of SOMA.

---

## 3 · Quantum incarnation

The three tongues map cleanly onto three quantization schemes:

| Tongue | Geometric object | Quantum dual |
|---|---|---|
| I — Intrinsic (lengths) | Cayley–Menger determinant | Hamiltonian eigenvalue spectrum |
| II — Extrinsic (vertices) | Shoelace integral | Wavefunction in a chosen basis |
| III — Topological (lattice) | Pick's $I + B/2 - 1$ | Chern number, Wilson loop, term symbol |

**Action quantization.** The Bohr–Sommerfeld condition $\oint p\, dq = (n + \tfrac{1}{2})\hbar$ is *exactly* a Shoelace integral around a phase-space loop. The semiclassical area of a closed orbit is the half-integer quantum number — Shoelace becomes spectrum.

**Berry curvature.** $\mathcal{F} = \mathrm{Im}\,\langle \partial_\mu \psi | \partial_\nu \psi \rangle$ integrated over a Brillouin zone is a Shoelace-type flux through a closed surface; the Chern number $C = \frac{1}{2\pi}\int \mathcal{F}$ is its Pick-counterpart — a *topological integer* that the continuous integral must equal.

**Quantum geometry tensor.** The 2026 SOTA work on flat-band superconductivity has crystallised the link between the *real* part of the quantum geometric tensor (the Fubini–Study metric) and superfluid weight: in flat bands, where conventional dispersion-driven supercurrent vanishes, the entire stiffness is *geometric* and admits a topological lower bound by the Chern number squared (Törmä–Peotta–Bernevig, *Nat. Rev. Phys.* 2022; see also recent work on quasicrystals where the metric in flux space replaces momentum-space metric, and on minimal-quantum-metric bounds in multi-orbital systems). This is the **Tongue II ↔ Tongue III** dictionary made physical: the metric (extrinsic) is bounded below by the integer (topological).

---

## 4 · Why three, and not two?

A profound feature of SOMA is that *no two tongues suffice*. Consider:

- **Lengths alone (I)** cannot distinguish a triangle from its mirror image, nor a flexible polygon from a rigid one. The Cayley–Menger machinery flags non-embeddability but cannot fix orientation.
- **Vertices alone (II)** cannot survive a coordinate change without extra data; rotated and translated copies need the metric to identify them.
- **Lattice census alone (III)** is metric-blind: Pick's formula gives the same number for arbitrarily distorted lattice polygons of equal $I$ and $B$.

It is the *closure of the triangle* that locks the invariant. This is why physical theories that try to live on only two corners — pure spectra, pure wavefunctions, or pure topological numbers — keep needing the third to compute observables.

> **Thought experiment.** A spectroscopist measures only intrinsic energies (Tongue I). A crystallographer measures only positions (Tongue II). A topologist measures only winding numbers (Tongue III). None of them, alone, can predict the conductance of a flat-band material. Combine all three and the prediction becomes overdetermined — and consistent. Overdetermination *is* the signature of a true invariant.

---

## 5 · The triality at higher order

The construction lifts:

- **Cayley–Menger** generalises Heron to $n$-simplex volumes via squared edge-distance determinants.
- **Stokes'** theorem generalises Shoelace to all closed forms on oriented manifolds.
- **Ehrhart polynomials** generalise Pick to lattice polytopes in any dimension; the leading coefficient is the volume, the next is half the surface area, and the constant term is the Euler characteristic — *all three tongues encoded in a single polynomial*.

The Ehrhart polynomial $L_P(t) = \mathrm{Vol}(P)\, t^d + \tfrac{1}{2}\mathrm{Vol}(\partial P)\, t^{d-1} + \dots + \chi(P)$ is, *literally*, SOMA written as one expression. Recent advances — graded $q$-Ehrhart series, weighted Ehrhart functions, Chapoton's refinements — extend the dictionary into representation theory and toric geometry, suggesting that the triality is in fact a *fragment* of a much richer algebraic structure.

---

## 6 · Energy as area

The deepest claim of SOMA: **energy, in its many guises, is an area-like quantity, and inherits the triality.**

- *Thermodynamic energy* lives on phase-space loops (Shoelace; Tongue II).
- *Spectral energy* lives in the Hamiltonian's intrinsic eigenstructure (Cayley–Menger-like; Tongue I).
- *Topological energy* — flat-band condensation, Chern insulators, fractional quantum Hall gaps — is bounded by integer counts (Pick-like; Tongue III).

The Hund exchange integral $K_{ar}$, which sets singlet–triplet gaps as $\Delta_{ST} = 2K_{ar}$, is computed as an *overlap area* between orbital densities — a Shoelace-type integral whose lower bound is set by spin algebra (a Pick-type integer count of unpaired electrons).

---

## 7 · Conclusions

1. The three classical area formulas are not three separate truths but three *projections* of a single invariant.
2. The same triality structures every area-like physical observable: action, Berry flux, exchange energy, superfluid weight.
3. Information-theoretically, no two tongues are sufficient; the *closure* of the dictionary triangle is the irreducible content of geometry.
4. The Ehrhart polynomial is the generating function of the entire triality and is the natural unifying object for further development.
5. Modern flat-band physics is the cleanest experimental laboratory for SOMA: there, the geometric (Tongue II) and topological (Tongue III) tongues become *directly measurable* through superfluid stiffness and Chern number bounds.

---

## Canonical references

Heron, *Metrica*, c. 60 CE. — Cayley, *On a theorem in the geometry of position*, 1841. — Menger, *Untersuchungen über allgemeine Metrik*, *Math. Ann.* 1928. — Pick, *Geometrisches zur Zahlenlehre*, 1899. — Ehrhart, *Sur les polyèdres rationnels homothétiques à n dimensions*, *C. R. Acad. Sci. Paris* 1962. — Provost & Vallee, *Riemannian structure on manifolds of quantum states*, *Comm. Math. Phys.* 1980. — Berry, *Quantal phase factors accompanying adiabatic changes*, *Proc. R. Soc.* 1984. — Törmä, Peotta, Bernevig, *Superconductivity, superfluidity and quantum geometry in twisted multilayer systems*, *Nat. Rev. Phys.* 4, 528 (2022). — Beck & Robins, *Computing the Continuous Discretely*, 2nd ed., Springer 2015.
