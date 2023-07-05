:::{math}
:nolabel:
\require{mhchem}
\require{physics}
:::

## Nucleus Basics
- The RMS radius of the proton is {math}`0.77\,\text{fm}`, radius of the nucleus approximately {math}`1.07 \cdot A^\frac{1}{3}\,\text{fm}`
- The surface thickness of the nucleus is approximately 2.4 fm (density drops from 90% to 10%).
- Between 1 fm and 20 fm, the strengths of the strong and coulomb interactions exchange places
   - Range of strong force known to be ~fm, because isotropic n-p scattering is **observed** ~ 10MeV in COM frame. Isotropic implies {math}`l<1` From {math}`\hbar l_\mathrm{max} = rp`, and {math}`p\approx\sqrt{2m_\mathrm{red}E}`. From this {cite:ps}`fetter_quantum_1972` it follows that {math}`r \sim \mathrm{fm}`
- 0.3% of the mass of an atom is _not_ in its nucleus
- room temperature ~eV vs nuclear reactions at ~MeV
- proton emission requires tunneling through coulomb barrier
  - what is intuition for this? 
- long-range forces not nearest neighbour (coulomb), long-range repulsion decreases B/A with A
  - 62 Ni most tightly bound

:::{note} To Do
- Coriolis Coupling?
- Cranking
- R process — rapid neutron capture followed by beta decay into less neutron-rich nuclei (higher Z)
- Binding energy, mass defect, mass deficit
- Isobaric analogue state
- Deformation model beta, phi — FONM p. 102 (Rowe)
- Selection rules
:::

## Nuclear forces
- Nuclear force is a residual effect of the fundamental strong interaction, mediated by gluons.
- Gluons partricipate in strong interaction in addition to mediating it;[^gluons] they carry (colour) charge
- Spin-orbit interaction phenomenological, reproduces magic numbers
  - Without spin-orbit, we can label single-particle states with {math}`\ket{ls;m_l m_s}`.
  - Spin-orbit interaction is of the form {math}`\mathbf{L}\cdot\mathbf{S}`, which is given by {math}`\mathbf{J}^2=\left(\mathbf{L}+\mathbf{S}\right)^2=\mathbf{L}^2+\mathbf{S}^2+2\mathbf{L}\cdot\mathbf{S}`. It doesn't commute with the spin operators {math}`\comm{\vb{L}\cdot\vb{S}}{\mathbf{L}_z} = -i\hbar \mathbf{L}_y`, but it does with {math}`\vb{J}^2` and {math}`\vb{J}_z`.
  - Under spin-orbit interaction, {math}`m_l` and {math}`m_s` are no longer good quantum numbers, so preferred basis becomes {math}`\ket{ls;jm_j}`.
  - For any spin-orbit doublet {math}`j = l \pm \frac{1}{2}`, the energy separation is {math}`\propto \expval{L\cdot S}`, with potential chosen such that larger {math}`j` is more tighly bound.
  - Lowering of high-{math}`j` leads to "intruder" states into lower shells with states of different parity (l) {cite:ps}`greiner_nuclear_1996`
  - {math}`s` states ({math}`l=0`) therefore are unpeturbed by the spin-orbit potential.
- What is spin-orbit, tensor?
- Charge symmetry - mirror nuclei
- Charge independence?[^np-scatter] np very similar cross section to pp, nn: difference due to {math}`\pi^\pm` meson exchange. Isobar triplets
- Isospin ~ good symmetry
- Spin (S) dependence of form {math}`S_1\cdot S_2` (deuteron unbound in S=0)
- Tensor component
  - For deuteron ground state to have mixed L in ground state, LS states can't be eigenstates of the Hamiltonian, i.e. there's a two-body tensor operator. Ultimate can be shown to have form {math}`V(r)S_{12}`[^np-scatter] {cite:ps}`fetter_quantum_1972`
- Relative velocity dependence
  <!-- S = S1 + S2, what is L -->
  - Of form {math}`V_\text{SO}L \cdot S`\bar
- Pairing interaction
  - Spatial overlap? Lookup existing notes on this
  - What does anti-aligned *mean*, is it z projections?
  - in even--even nuclei there is an energy gap of 1-2 MeV between the ground state and the lowest single-particle excitation. {cite:ps}`greiner_nuclear_1996`
- Mean field calculations fail to reproduce nuclear density without three-body forces {cite:ps}`rowe_fundamentals_2010`. It's not clear whether this is an artefact of the imposition of a single-slater determinant constraint on the ground state, vs a requirement at a fundamental level.
### Semi Empirical Mass Formula
A "liquid-drop" model, with surface, volume, pairing, coulbomb, and asymmetry terms
- Volume: _base-term_, short-range of residual strong force suggests nearest-neighbour model; saturation implies that this is modelled by a proportionality constant {math}`\propto a_V A`. Smaller than the nearest-neighbour binding energy, because some energy is required for kinetic energy, which increases with {math}`A` due to the Pauli exclusion principle (this can be determined by modelling the nucleus as a Fermi ball, and computing the kinetic energy of the non-interacting system).
- Surface: _subtractive_, at the surface, the nearest neighbour assumption breaks down, so we correct for it {math}`\propto a_S A^\frac{2}{3}`.
- Coulomb: _subtractive_, repulsion from proton {math}`\propto \frac{z(z-1)}{A^\frac{1}{3}}`, by assembling a sphere of uniform charge.
- Asymmetry: _subtractive_, Pauli exclusion principle precludes lower-energy orbits, therefore asymmetric nuclei have greater occupation of higher-energy orbits. This corresponds to increased energy {math}`\propto \pqty{N-Z}^2`, which derives from the kinetic energy of the Fermi ball (ignoring the contribution to the volume term).
- Pairing: _additive_, even numbers of nucleons can pair to spin-zero, enhanceing the binding through the overlap of same-j wavefunctions (different magnetic substates). Binding effect {math}`\propto a_P A^\frac{-1}{2} f(A, Z)`, where {math}`f(A,Z)` selects for even-z, even-n.

Binding energy per nucleon is fairly constant ~8MeV/nucleon for many A, meaning that the screening effect is significant / range of internucleon force << size of nucleus
  - Short range forces are nearest-neighbours in many body system
  - Surface effects dominate at small sizes & B/A decreases for light nuclei

## Shell Structure

- Nuclear shell structure arises because of the Pauli exclusion principle, prohibiting strong scattering of nucleons inside the nucleons by preventing scatering into orbitals already occupied.
  - What is "strong scattering"?
  - Find existing notes on this? Thesis?
- Magic numbers: 2, 8, 20, 28, 50, 82, 126
    - Doubly Magic nuclei:
      - {math}`\ce{^4 He}` — {math}`2(2)`
      - {math}`\ce{^16 O}` — {math}`2(8)`
      - {math}`\ce{^40 Ca}` — {math}`2(20)`
      - {math}`\ce{^56 Fe}` — {math}`2(28)`

## Rotor Model
- {math}`M` is the space-fixed {math}`\hat{z}` projection
- {math}`K` is the space-fixed {math}`\hat{3}` symmetry-axis projection

## TexAT
- Cyclotron? http://www.damtp.cam.ac.uk/user/tong/pp/pp3.pdf
- Gas cell?
- 

[^np-scatter]: https://ns.ph.liv.ac.uk/PHYS490/Phys490_latex.pdf
[^gluons]: https://en.wikipedia.org/wiki/Gluon#Eight_colors