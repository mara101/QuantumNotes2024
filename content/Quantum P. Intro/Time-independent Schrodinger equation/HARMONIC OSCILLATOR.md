
In this section, we explore the properties and solutions of the quantum harmonic oscillator. This model is essential in quantum mechanics because it exemplifies the principles of quantized energy levels, ladder operators, and the concept of tunneling into classically forbidden regions.
### Introduction to Discretized Spectra and the Harmonic Oscillator

We begin by recalling the previous discussion on discretized spectra: whenever a potential energy function $U(x)$ tends to infinity at large values of $x$ (typically as $x \to \pm \infty$), the energy spectrum of a particle moving within this potential becomes quantized. This means that the particle can only possess discrete energy values rather than a continuous range of energies, as seen in classical mechanics. In this lecture, we explore this behavior in the specific case of the **quantum harmonic oscillator**—a paradigmatic model in quantum mechanics with widespread applications.

The quantum harmonic oscillator not only exhibits quantized energy levels, but it also provides an example of [[BOUND STATES, SCATTERING STATES AND THE TUNNELING EFFECT|quantum tunneling]], where there is a non-zero probability of the particle penetrating into regions that are classically forbidden (where the particle’s total energy is less than the potential energy).

### The Classical Harmonic Oscillator

Classically, the harmonic oscillator can be described as a mass $m$ attached to an ideal spring with elastic constant $k$. According to **Hooke’s law**, the restoring force acting on the mass is proportional to its displacement from the equilibrium position:

$$F = -kx$$

Applying Newton’s second law, $F = ma$, gives the following differential equation for the motion of the mass:

$$m \frac{d^2 x}{dt^2} + kx = 0$$

The general solution to this equation is:

$$x(t) = A \cos(\omega t) + B \sin(\omega t)$$

where $\omega = \sqrt{\frac{k}{m}}$ is the angular frequency of the oscillator, and $A$ and $B$ are constants determined by the initial conditions. The motion of the oscillator is periodic, with the potential energy given by:

$$U(x) = \frac{1}{2} k x^2 = \frac{1}{2} m \omega^2 x^2$$

The total energy $E$ of the oscillator is conserved and is the sum of the potential and kinetic energy. The kinetic energy is maximized when the mass passes through the equilibrium position $x = 0$, and it vanishes at the turning points where the mass changes direction.

At the turning points, the total energy is purely potential:

$$E = \frac{1}{2} k x^{*2}$$

Thus, the motion is confined between two turning points, $\pm x^*$, where the spring reaches its maximum extension.

### The Quantum Harmonic Oscillator

In the quantum mechanical version of the harmonic oscillator, we describe the system using the **Schrödinger equation**. The Hamiltonian operator for the quantum harmonic oscillator is given by:

$$\hat{H}_{\text{HO}} = -\frac{\hbar^2}{2m} \frac{d^2}{dx^2} + \frac{1}{2} m \omega^2 x^2$$

This Hamiltonian consists of a kinetic energy term (represented by the second derivative with respect to $x$) and a potential energy term (proportional to $x^2$). The potential energy increases quadratically as $x \to \pm \infty$, which confines the particle to a finite region of space.

#### Energy Quantization

Since the potential energy tends to infinity as $x \to \pm \infty$, the particle cannot move beyond these limits, and its energy must be greater than the potential energy only within a finite region. As a result, the energy spectrum is **quantized**, meaning the particle can only occupy discrete energy levels. This is in contrast to the continuous spectrum that might be found in a free particle or a particle in a potential well with finite walls.

To determine the energy levels of the harmonic oscillator, we solve the time-independent Schrödinger equation. Several methods can be used, including the **power expansion method**, which identifies the solutions as the well-known **Hermite polynomials**. However, a more elegant and widely applicable approach involves the use of **ladder operators**.

### Solution with Ladder Operators

To simplify the solution, we can express the Hamiltonian in a quadratic form. We introduce two constants, $p_0 = \sqrt{2\hbar m \omega}$ and $x_0 = \sqrt{\frac{\hbar}{m \omega}}$, which allow us to write the Hamiltonian in a dimensionless form:

$$\hat{H}_{\text{HO}} = \hbar \omega \left( \frac{p^2}{p_0^2} + \frac{x^2}{x_0^2} \right)$$

Next, we define the ladder (or creation and annihilation) operators, $\hat{a}$ and $\hat{a}^\dagger$, which combine the position and momentum operators:

$$\hat{a} = \frac{x}{x_0} + i \frac{p}{p_0}, \quad \hat{a}^\dagger = \frac{x}{x_0} - i \frac{p}{p_0}$$

The Hamiltonian can then be written in terms of these operators:

$$\hat{H}_{\text{HO}} = \hbar \omega \left( \hat{a}^\dagger \hat{a} + \frac{1}{2} \right)$$

These operators have the crucial property that they allow us to "raise" or "lower" the energy of a quantum state by one quantum of energy $\hbar \omega$. The operator $\hat{a}$ lowers the energy of a state, while $\hat{a}^\dagger$ raises the energy:

$$[H, \hat{a}] = -\hbar \omega \hat{a}, \quad [H, \hat{a}^\dagger] = \hbar \omega \hat{a}^\dagger$$
### Understanding the Commutation Relations

The Hamiltonian for the quantum harmonic oscillator is given by:

$$H = \hbar \omega \left( \hat{a}^\dagger \hat{a} + \frac{1}{2} \right)$$

This describes the energy of the system, where $\hat{a}^\dagger \hat{a}$ is the **number operator** that counts the number of quanta (or phonons) in the state.

Now, consider the commutation relations:

$$[H, \hat{a}] = -\hbar \omega \hat{a}, \quad [H, \hat{a}^\dagger] = \hbar \omega \hat{a}^\dagger$$

#### Why Do These Commutators Indicate Raising and Lowering of Energy?

##### Lowering the Energy with $\hat{a}$

The first commutation relation, $[H, \hat{a}] = -\hbar \omega \hat{a}$, tells us what happens when $\hat{a}$ acts on a state. 

Suppose we have a quantum state $|\psi\rangle$ with an energy eigenvalue $E$, meaning that:

$$H |\psi\rangle = E |\psi\rangle$$

Now, let's consider the effect of applying $\hat{a}$ to this state. Using the commutation relation:

$$H (\hat{a} |\psi\rangle) = (\hat{a} H + [H, \hat{a}]) |\psi\rangle$$

Substituting the commutator $[H, \hat{a}] = -\hbar \omega \hat{a}$:

$$H (\hat{a} |\psi\rangle) = \hat{a} H |\psi\rangle - \hbar \omega \hat{a} |\psi\rangle$$

Since $H |\psi\rangle = E |\psi\rangle$, we have:

$$H (\hat{a} |\psi\rangle) = \hat{a} E |\psi\rangle - \hbar \omega \hat{a} |\psi\rangle$$

$$H (\hat{a} |\psi\rangle) = (E - \hbar \omega) (\hat{a} |\psi\rangle)$$

Thus, $\hat{a} |\psi\rangle$ is an eigenstate of the Hamiltonian with an energy eigenvalue reduced by $\hbar \omega$. This shows that applying $\hat{a}$ to a state **lowers** the energy of that state by one quantum of energy $\hbar \omega$.

##### Raising the Energy with $\hat{a}^\dagger$

Similarly, the second commutation relation, $[H, \hat{a}^\dagger] = \hbar \omega \hat{a}^\dagger$, tells us how $\hat{a}^\dagger$ acts on a state.

If we apply $\hat{a}^\dagger$ to a state $|\psi\rangle$, we get:

$$H (\hat{a}^\dagger |\psi\rangle) = (\hat{a}^\dagger H + [H, \hat{a}^\dagger]) |\psi\rangle$$

Substituting the commutator $[H, \hat{a}^\dagger] = \hbar \omega \hat{a}^\dagger$:

$$H (\hat{a}^\dagger |\psi\rangle) = \hat{a}^\dagger H |\psi\rangle + \hbar \omega \hat{a}^\dagger |\psi\rangle$$

Again, since $H |\psi\rangle = E |\psi\rangle$:

$$H (\hat{a}^\dagger |\psi\rangle) = \hat{a}^\dagger E |\psi\rangle + \hbar \omega \hat{a}^\dagger |\psi\rangle$$

$$H (\hat{a}^\dagger |\psi\rangle) = (E + \hbar \omega) (\hat{a}^\dagger |\psi\rangle)$$

Thus, $\hat{a}^\dagger |\psi\rangle$ is an eigenstate of the Hamiltonian with an energy eigenvalue **increased** by $\hbar \omega$. This shows that applying $\hat{a}^\dagger$ to a state **raises** its energy by one quantum of energy $\hbar \omega$.


This process constructs a **ladder** of energy levels, with each step separated by $\hbar \omega$. The ladder cannot extend infinitely in the negative direction because energy must be positive, so there is a minimum energy state, known as the **ground state**.

### The Ground State and Excited States

The ground state, denoted $|\psi_0 \rangle$, is the state that cannot be lowered any further by the annihilation (lowering) operator $\hat{a}$. This means:

$$\hat{a} |\psi_0 \rangle = 0$$

In this case, $\hat{a}$ annihilates the ground state, making it the lowest possible energy state. To find the explicit form of the ground state, we solve this equation in the position representation. The operator $\hat{a}$, in terms of position and momentum, is given by:

$$\hat{a} = \frac{x}{x_0} + i \frac{p}{p_0}$$

Substituting this into the condition $\hat{a} |\psi_0 \rangle = 0$, we obtain a first-order differential equation for the ground state wavefunction. Solving this equation yields the ground state wavefunction in the position representation:

$$\psi_0(x) = C e^{-\frac{x^2}{2x_0^2}}$$

This is a Gaussian wavefunction, where $x_0 = \sqrt{\frac{\hbar}{m \omega}}$ is the characteristic length scale of the harmonic oscillator. The constant $C$ is determined by normalization:

$$C = \frac{1}{\sqrt{x_0 \sqrt{\pi}}}$$

Importantly, the ground state energy is not zero, but rather:

$$E_0 = \frac{1}{2} \hbar \omega$$

This non-zero ground state energy is a result of the **Heisenberg uncertainty principle**, which prevents both the position and momentum of the particle from being exactly zero. Even in the lowest energy state, the particle retains some "zero-point" motion, leading to a ground state energy greater than zero.

### Excited States and Hermite Polynomials

The excited states of the harmonic oscillator can be generated by repeatedly applying the raising operator $\hat{a}^\dagger$ to the ground state. This is why $\hat{a}^\dagger$ is known as the creation (raising) operator, as it increases the energy of a state by one quantum of energy $\hbar \omega$.

The $n$-th excited state is given by:

$$|\psi_n \rangle = \frac{(\hat{a}^\dagger)^n}{\sqrt{n!}} |\psi_0 \rangle$$

In the position representation, these excited states have the form:

$$\psi_n(x) = H_n \left( \frac{x}{x_0} \right) \psi_0(x)$$

Here, $H_n(x)$ are the **Hermite polynomials** of degree $n$, and $\psi_0(x)$ is the Gaussian ground state wavefunction. Each excited state corresponds to a higher quantized energy level:

$$E_n = \hbar \omega \left( n + \frac{1}{2} \right)$$

The energy levels are equally spaced by $\hbar \omega$, with the ground state having an energy of $E_0 = \frac{1}{2} \hbar \omega$ and the first excited state having an energy of $E_1 = \frac{3}{2} \hbar \omega$, and so on.

### Penetration into Classically Forbidden Regions

An important feature of these quantum states is that the probability density of the particle extends into the **classically forbidden region**—where the potential energy exceeds the total energy. In classical mechanics, the particle would be confined between the turning points (where its total energy equals its potential energy). However, in quantum mechanics, the wavefunction (and hence the probability density) has non-zero values even in regions where $U(x) > E_n$.

For example, the ground state wavefunction $\psi_0(x)$ decays exponentially outside the classically allowed region, with the behavior:

$$\psi_0(x) \propto e^{-\frac{x^2}{2x_0^2}}$$

This exponential decay illustrates the phenomenon of [[BOUND STATES, SCATTERING STATES AND THE TUNNELING EFFECT|quantum tunneling]], where there is a non-zero probability of finding the particle in regions that are forbidden by classical physics.



