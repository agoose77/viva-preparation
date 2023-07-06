:::{math}
:nolabel:
\require{mhchem}
\require{physics}
:::

## Nucleus Basics
- The RMS radius of the proton is {math}`0.77\,\text{fm}`, radius of the nucleus approximately {math}`1.27 \cdot A^\frac{1}{3}\,\text{fm}`
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
  - Lowering of high-{math}`j` leads to "intruder" states into lower shells with states of different parity (due to l) and angular momentum {cite:ps}`greiner_nuclear_1996`. These states tend to be long-lived, as the transition probabilities to the ground state are correspondingly small.
  - {math}`s` states ({math}`l=0`) therefore are unpeturbed by the spin-orbit potential.
- Spin (S) dependence of form {math}`S_1\cdot S_2` (deuteron unbound in S=0)
- Tensor component
  - For deuteron ground state to have mixed L in ground state, LS states can't be eigenstates of the Hamiltonian, i.e. there's a two-body tensor operator. Ultimately can be shown to have form {math}`V(r)S_{12}`[^np-scatter] {cite:ps}`fetter_quantum_1972`
  - Believe that we handle tensor component in residual interaction (non-diagonal), so we talk about states in terms of central-potential eigenstates.
- Charge symmetry - mirror nuclei
- Charge independence?[^np-scatter] np very similar cross section to pp, nn: difference due to {math}`\pi^\pm` meson exchange. Isobar triplets. Discrepancy noticed in small difference between charged and neutral pions masses.
- Isospin ~ good symmetry
- Relative velocity dependence
  <!-- S = S1 + S2, what is L -->
  - Of form {math}`V_\text{SO}L \cdot S`
- Pairing interaction
  - Spatial overlap? Lookup existing notes on this
  - What does anti-aligned *mean*, is it z projections?
  - in even--even nuclei there is an energy gap of 1-2 MeV between the ground state and the lowest single-particle excitation. {cite:ps}`greiner_nuclear_1996`
  - Pairing can also be seen as an odd–even effect, relating to the masses of even–even and odd-A nuclei. Experiment has established that the total binding energy of an odd-A nucleus is less than the average of the total binding energies of the two neighbouring even–even nuclei. {cite:ps}`suhonen_nucleons_2007`
  - experimentally most open-shell nuclei are spherical in their low-lying states. The explanation is that the short-range pairing interaction favours spherical symmetry and maintains the spherical shape rather far into the open shell. {cite:ps}`suhonen_nucleons_2007`
  - Prolate nuclei near beginning of major shell, due to pairing preferentially populating large {math}`\abs{m}` states
  - Only pp, nn because deuteron is J=1, not J=0
- Mean field calculations fail to reproduce nuclear density without three-body forces {cite:ps}`rowe_fundamentals_2010`. It's not clear whether this is an artefact of the imposition of a single-slater determinant constraint on the ground state, vs a requirement at a fundamental level.
- Free-nucleon interactions are generally much too strong at short distances for diret use in the shell model (too slow convergence in shell model) - infinite matrix elements for hard core.
   - Phenomenologically the short-range hard repulsion is compensated for by strong attractive components; hence shell model. Effective potentials are simplifications of the system that suppress short-range correlations p. 266 FONM

### Deuteron 
- Binding energy of 2.225 MeV
- No excited bound states
- Observed to have {math}`J^\pi=1^+`
- Parity of nucleus is {math}` \pi_L \pi_\text{intr} =-1^L\times (+)` (product of total orbital angular momentum parity and total intrinsic parity)
   - {math}`L\in \Bqty{0, 2, 4, ...}`
- {math}`LS` coupling gives {math}`\abs{L-S} \leq J \leq L+S`: {math}`\ket{L S} \in \Bqty{\ket{01}, \ket{21}}` - TODO, what are the coupling coefficients?
   - {math}`S=1`
- {math}`L=0` state is dominant
- Observed isospin projection of deuteron is {math}`T_z=\frac{-1}{2}+\frac{1}{2}=0`, and {math}`\vb{T}_1+\vb{T}_2` must therefore couple to either {math}`\ket{TT_z}=\ket{00}` or {math}`\ket{TT_z}=\ket{10}`.
- Under _exchange_, wavefunction must be antisymmetric. {math}`P_SP_TP_r=-1`. {math}`P_r` given by parity (exchange equivalent to parity change for spherical harmonics). {math}`P_S` is symmetric for {math}`S=1`, which can be shown by constructing top rung (symmetric), and lowering with (symmetric) {math}`S_-` operator. Hence, {math}`P_T` must be antisymmetric, i.e. {math}`T=0`.
- Or, there's no dineutron so {math}`T=1` is unlikely. Therefore, {math}`T=0`.
- The existence of a nonvanishing quadrupole moment (requiring L>0) is direct evidence of the presence of the 3D1-component
in the deuteron ground state. 
% Intrinsic parity of p,n same as considered +1 (due to three quarks?)

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

Matter distribution inferred by charge distribution from electron scattering.

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
- Woods Saxon potential {math}`V(r)=\frac{-V_0}{1+\exp\pqty{\frac{r-R}{a}}}`
  - Surface diffuseness {math}`a=0.67` fm
  - Nuclear radius {math}`1.27 A^\frac{1}{3}` fm
  - Potential {math}`V_0=57` MeV
- Harmonic oscillator potential {math}`V(r) = -V_1 + \frac{1}{2}m\omega^2 r^2`
  - :::{figure} https://upload.wikimedia.org/wikipedia/commons/9/9e/HarmOsziFunktionen.png
    :::
- Prediction of states:
    - Odd-even — last unpaired nucleon
    - Even-even — pairing to J=0
    - Odd-odd — couple JJ as even-even core + p + n, range of candidates
## Rotor Model
- {math}`M` is the space-fixed {math}`\hat{z}` projection
- {math}`K` is the space-fixed {math}`\hat{3}` symmetry-axis projection

## Angular Momentum
- :::{math}
  \begin{aligned}
  J_{+}\ket{j, m} &=\sqrt{(j-m)(j+m+1)} \hbar\ket{j, m+1}  \\
  J_{-}\ket{j, m} &=\sqrt{(j+m)(j-m+1)} \hbar\ket{j, m-1} .
  \end{aligned}
  :::
- :::{math}
  \begin{aligned}
  2\vb{J}_1\cdot\vb{J}_2 = 2 J_{1 z} J_{2 z}+J_{1+} J_{2-}+J_{1-} J_{2+}
  \end{aligned}
  :::
- :::{math}
  \begin{aligned}
  J_- = J_x - iJ_y
  \end{aligned}
  :::

## TexAT
- Cyclotron? http://www.damtp.cam.ac.uk/user/tong/pp/pp3.pdf
- Gas cell?

## Scattering
- Rutherford scattering is minimal for 180° in the CoM frame
    :::{math}
    \dv{\sigma}{\Omega} =
    \pqty{
        \frac{Z_1 Z_2 e^2}{4 \pi \epsilon_o}
    }^2
    \pqty{
        \frac{1}{4 E_{c . m .}}
    }^2
        \pqty{\frac{1}{\sin ^4 \frac{\theta_{c . m .}}{2}}
    }
    :::

[^np-scatter]: https://ns.ph.liv.ac.uk/PHYS490/Phys490_latex.pdf
[^gluons]: https://en.wikipedia.org/wiki/Gluon#Eight_colors