In this note we will discuss why in quantum mechanics sometimes we have discrete energy levels and why other times we have continuous one.

In quantum mechanics, the difference between discrete energy levels in systems like the [[THE INFINITE SQUARE WELL|infinite well]] and the continuous energy spectrum for the [[THE FREE PARTICLE|the free particle]] comes from the boundary conditions and the nature of the system. Below, we explore why these two cases behave differently.
## Quantum Well: Discrete Energy Levels

In a **quantum well** (also known as a particle in a box), the particle is confined to a specific region of space. This confinement introduces **boundary conditions** that the wave function must satisfy. For example, in a one-dimensional infinite quantum well, the potential energy is zero inside the well and infinite outside. The particle cannot exist outside the well, so the wave function $\psi(x)$ must vanish at the boundaries (typically at $x = 0$ and $x = L$ for a well of width $L$).

The time-independent Schrödinger equation for a quantum well is:

$$
-\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} = E \psi(x)
$$

The boundary conditions ($\psi(0) = 0$ and $\psi(L) = 0$) force the wave function to take the form of sine waves that fit perfectly within the well. These allowed wave functions are:

$$
\psi_n(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{n\pi x}{L}\right), \quad n = 1, 2, 3, \dots
$$

where $n$ is a positive integer known as the **quantum number**.

These boundary conditions lead to quantized values of energy. The energy levels are given by:

$$
E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}, \quad n = 1, 2, 3, \dots
$$

Thus, the energy of the particle is **discrete** because only certain wavelengths (and therefore certain energies) can fit within the boundaries of the well. This quantization arises from the constraints imposed by the spatial confinement.

## Free Particle: Continuous Energy and Wave Packets

In contrast, a **free particle** is not confined to any region of space, meaning it can move freely throughout all space without any boundary conditions. The potential energy $V(x)$ is zero everywhere, and the Schrödinger equation becomes:

$$
-\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} = E \psi(x)
$$

The solutions to this equation are **plane waves** of the form:

$$
\psi(x) = Ae^{ikx} + Be^{-ikx}
$$

where $k = \sqrt{\frac{2mE}{\hbar^2}}$ is related to the energy and momentum of the particle. These plane waves describe particles with any possible value of momentum $p = \hbar k$ and energy $E = \frac{\hbar^2 k^2}{2m}$. There are **no boundary conditions** restricting the values of $k$, so the particle's energy is **continuous** and can take any positive value.

However, these plane wave solutions are not normalizable over infinite space because their probability density $|\psi(x)|^2$ does not go to zero as $x \to \infty$. To describe a physical free particle, we use **wave packets**, which are superposition of plane waves with different wave numbers (and hence different energies). A wave packet is a localized wave function that can be written as:

$$
\psi(x, t) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \phi(k) e^{i(kx - \frac{\hbar k^2}{2m}t)} dk
$$

Here, $\phi(k)$ is a distribution of wave numbers, which allows the particle to be localized in space. Since the wave packet is made up of a continuous range of $k$ values, the corresponding energies form a **continuous spectrum**.
## Eigenfunctions of a Hermitian Operator

In quantum mechanics, [[OBSERVABLE IN HILBERT SPACE, HERMITIAN OPERATORS AND UNITARY OPERATORS|observable]] are represented by **Hermitian operators**, which have eigenfunctions corresponding to physically measurable values (eigenvalues). These eigenfunctions describe the possible states that a quantum system can occupy when a measurement of the observable is made. Depending on the system, the spectrum of eigenvalues can be either **discrete** or **continuous**. 
### Discrete Spectrum

For Hermitian operators with a **discrete spectrum**, the eigenfunctions have the following key properties:

1. **Eigenvalues are Real**: Since Hermitian operators correspond to physical observables, their [[EIGENVALUES AND EIGENFUNCTIONS|eigenvalues]] are real. If $Q$ is a Hermitian operator, and $Q\psi = q\psi$, where $\psi$ is an eigenfunction and $q$ is the corresponding eigenvalue, then $q$ is always real. This guarantees that measurements of physical quantities result in real values.

2. **Eigenfunctions are Orthogonal**: If $Q$ is a Hermitian operator, the eigenfunctions associated with different eigenvalues are orthogonal. If $\psi_n$ and $\psi_m$ are eigenfunctions corresponding to eigenvalues $q_n$ and $q_m$ respectively, and $q_n \neq q_m$, then:

   $$
   \langle \psi_n | \psi_m \rangle = 0
   $$

   This orthogonality is crucial in constructing a complete set of basis functions for representing quantum states.

3. **Completeness**: The set of eigenfunctions corresponding to a Hermitian operator forms a **complete basis** in the Hilbert space. This means that any state in the space can be written as a linear combination of the operator’s eigenfunctions. Mathematically, any state $\psi(x)$ can be expanded as:

   $$
   \psi(x) = \sum_n c_n \psi_n(x)
   $$

   where $c_n$ are the expansion coefficients. Completeness ensures that the eigenfunctions span the entire space of possible quantum states.
### Continuous Spectrum

In contrast to the discrete case, Hermitian operators can also have a **continuous spectrum**, where the eigenvalues fill an entire range without gaps. This situation arises when the system is not confined to a finite region, as in the case of a **free particle**. In this case, the eigenfunctions are not normalizable in the usual sense, but they still satisfy a special kind of orthogonality, called **Dirac orthogonality**.
#### Dirac Orthogonality

In the continuous spectrum, the eigenfunctions are not square-integrable over all space, meaning their integral over all space diverges. For example, the eigenfunctions of the **momentum operator** in position space are plane waves of the form:

$$
\psi_p(x) = \frac{1}{\sqrt{2\pi \hbar}} e^{ipx/\hbar}
$$

These plane waves extend infinitely and cannot be normalized in the usual way (i.e., $\int |\psi_p(x)|^2 dx = \infty$). However, they still satisfy a form of orthogonality known as **Dirac orthogonality**. Instead of the discrete Kronecker delta for orthogonality, the continuous eigenfunctions use the **Dirac delta function** $\delta(p - p')$:

$$
\langle \psi_p | \psi_{p'} \rangle = \delta(p - p')
$$

This means that the momentum eigenfunctions are orthogonal in the sense that they are only "overlapping" when $p = p'$. The Dirac delta function acts as a generalized version of orthogonality for continuous spectra, ensuring that different momentum eigenfunctions correspond to distinct momentum states.

#### Properties of Dirac Orthogonality

1. **Non-normalizability**: Continuous spectrum eigenfunctions are not square-integrable over all space, so they cannot be normalized in the usual sense. For example, the plane waves for a free particle extend over infinite space and do not vanish at infinity, so their norm is infinite.

2. **Dirac Delta Function**: Orthogonality in the continuous case is represented by the Dirac delta function:

   $$
   \langle \psi_p | \psi_{p'} \rangle = \delta(p - p')
   $$

   This delta function expresses that eigenfunctions are only orthogonal when evaluated at different eigenvalues, and are not localized in the usual sense. The delta function has the property that:

   $$
   \int_{-\infty}^{\infty} \delta(p - p') dp = 1
   $$

   This ensures that when we integrate over the continuous spectrum, we properly account for the "orthogonality" of different momentum eigenfunctions.

3. **Completeness**: Just as with discrete spectra, the continuous spectrum eigenfunctions form a complete set. However, instead of summing over discrete eigenfunctions, we integrate over the continuous set of eigenfunctions. Any wave function can be expressed as a superposition (integral) of momentum eigenfunctions:

   $$
   \psi(x) = \int_{-\infty}^{\infty} c(p) \psi_p(x) dp
   $$

   where $c(p)$ are the expansion coefficients in terms of momentum eigenfunctions. This completeness ensures that even in the continuous case, any quantum state can be represented using these eigenfunctions.

