## OBSERVABLE
Observable in quantum mechanics as we have just seen in the [[THE UNCERTAINTY PRINCIPLE|uncertainty principle]] cannot be represented by numbers and so we have to find another mathematical tool to represent them. This type of tool is called *Hermitian Operator*. Those types of operators are part of [[CONNECTIONS WITH LINEAR ALGEBRA AND HILBERT SPACE|Hilbert space]].

The expectation value of a general observable $Q$ is expressed as such:
![[Screenshot_20241004_110540.png]]

Now even if the observable could not be represented by a value it's expectation value has to be a real value so it follows the property:
![[Screenshot_20241004_110900.png]]
If the complex conjugate of the operator does not change it follows also that
you can change the order of operation on the wave function $\psi$:
![[Screenshot_20241004_111318.png]]

## Definition of a Hermitian Operator

A fundamental concept in quantum mechanics is the **Hermitian operator**. An operator $\hat{A}$ is called **Hermitian** if it satisfies a specific condition that relates two quantum states $|\psi\rangle$ and $|\phi\rangle$ in a Hilbert space. This condition is:

$$
\langle \psi | \hat{A} \phi \rangle = \langle \hat{A} \psi | \phi \rangle
$$

This relation implies that the action of $\hat{A}$ on $|\psi\rangle$ behaves the same as taking the adjoint (complex conjugate transpose) of $\hat{A}$ and acting on $|\phi\rangle$. In other words, the operator $\hat{A}$ is equal to its **adjoint**:

$$
\hat{A}^\dagger = \hat{A}
$$

Here, $\hat{A}^\dagger$ denotes the **adjoint** of $\hat{A}$, which is the operator obtained by taking the complex conjugate and transposing $\hat{A}$.

### Key Properties of Hermitian Operators

Hermitian operators have several important properties that are crucial in quantum mechanics:

1. **Real Eigenvalues**:  
   A defining feature of Hermitian operators is that their [[EIGENVALUES AND EIGENFUNCTIONS|eigenvalues]] are always real. This is particularly significant because, in quantum mechanics, the eigenvalues of operators correspond to measurable quantities (observables), which must be real, as we seen above.

2. **Orthogonality of Eigenvectors**:  
   The eigenvectors corresponding to different eigenvalues of a Hermitian operator are orthogonal. If $|\psi_1\rangle$ and $|\psi_2\rangle$ are eigenvectors with different eigenvalues, their inner product vanishes:
   $$
   \langle \psi_1 | \psi_2 \rangle = 0
   $$
   This orthogonality property is essential in constructing a complete set of states for a quantum system.

3. **Spectral Theorem**:  
   The **spectral theorem** states that any Hermitian operator can be diagonalized in an orthonormal basis. This means that the operator can be represented as a diagonal matrix, with its real eigenvalues appearing along the diagonal. This property is foundational in quantum mechanics because it allows us to decompose quantum states into a sum of eigenstates of an observable, each corresponding to a distinct measurement outcome.
### Example of a Hermitian Operator

One of the most prominent examples of a Hermitian operator in quantum mechanics is the **Hamiltonian** $\hat{H}$, which represents the total energy of a quantum system. Since the Hamiltonian is Hermitian, its eigenvalues—representing the possible energy levels of the system—are guaranteed to be real, ensuring that measured energy values are physically meaningful.

Other examples of Hermitian operators include the **position operator** $\hat{x}$ and the **momentum operator** $\hat{p}$. These operators, when expressed in appropriate bases (such as the position or momentum representation), are Hermitian, ensuring that measurements of position and momentum yield real values.
## Unitary Operators
In quantum mechanics, we frequently encounter complicated eigenfunctions coexisting with simple energy spectra. This often points to an underlying **symmetry** in the physical system. For example, in the cases we’ve studied, like the [[THE FREE PARTICLE|free particle]] or the [[HARMONIC OSCILLATOR|harmonic oscillator]], symmetry plays a crucial role in simplifying the solution of the Schrödinger Equation. These systems exhibit symmetry in the exchange of position $x$ and momentum $p$, even though the position and momentum operators themselves do not share this symmetry in configuration or momentum space.

When solving the Time-Independent Schrödinger Equation, it is sometimes more efficient to choose a basis that captures the symmetries of the system rather than using a continuous basis like $\{|x\rangle\}$ or $\{|p\rangle\}$. For example, in the harmonic oscillator, we used the [[PHONONS|Fock Space]], which consists of the eigenstates of the number operator. These eigenstates simplify the problem even when dealing with an anharmonic oscillator, which introduces small deviations from the harmonic potential.

### Changing Basis

In quantum mechanics, a quantum state $|\Psi(t)\rangle$ is a vector in an infinite-dimensional [[CONNECTIONS WITH LINEAR ALGEBRA AND HILBERT SPACE|Hilbert Space]]. This vector can be represented as a superposition of unit basis vectors from various possible bases. For example, when solving the eigenvalue problem of the harmonic oscillator, we found a complete, orthonormal set of eigenstates that simplified the Hamiltonian into a diagonal form. Even in more complex problems, such as the anharmonic oscillator, it is often advantageous to express the Hamiltonian in terms of a different basis that reflects the system's symmetries.

A **change of basis** between two complete orthonormal sets of states $\{|\psi_n\rangle\}$ and $\{|\tilde{\psi}_n\rangle\}$ can be described by a **unitary operator** $U$. The relationship between the old and new basis is given by:

$$
|\tilde{\psi}_n\rangle = U |\psi_n\rangle
$$

To preserve the normalization of the basis states, $U$ must satisfy:

$$
U^\dagger = U^{-1}
$$

This defines a **unitary operator**, whose adjoint (conjugate transpose) is also its inverse. One important consequence of this property is that unitary operators preserve inner products and probabilities in quantum mechanics.

### Impact on Operators: Unitary Transformation

When we change the basis in which a quantum system is described, the operators representing physical observables, such as the Hamiltonian, must also transform consistently. If we apply a unitary transformation to the system's basis, the corresponding operator $\hat{O}$ transforms as:

$$
\tilde{O} = U \hat{O} U^\dagger = U \hat{O} U^{-1}
$$

This ensures that the transformed operator $\tilde{O}$ still represents the same physical observable in the new basis. Importantly, the **expectation values** of the operator must remain the same in both bases:

$$
\langle \tilde{\psi} | \tilde{O} | \tilde{\psi} \rangle = \langle \psi | \hat{O} | \psi \rangle
$$

Thus, unitary transformations do not affect the physical measurement results.

### Unitary Transformations and Eigenvalues

A unitary transformation does not alter the **eigenvalues** of an operator. For instance, consider the Hamiltonian operator $\hat{H}$. When we transform it into a new basis, its eigenvalues remain the same because the expectation value is preserved. This can be seen in the following expression:

$$
\tilde{H}|\tilde{\psi}_n\rangle = E_n |\tilde{\psi}_n\rangle \quad \Rightarrow \quad U\hat{H}U^{-1} U|\psi_n\rangle = E_n U|\psi_n\rangle \quad \Rightarrow \quad \hat{H}|\psi_n\rangle = E_n|\psi_n\rangle
$$

Thus, solving the Schrödinger equation often involves finding a **unitary transformation** that diagonalizes the Hamiltonian operator, simplifying the problem by rotating it into a diagonal form where the eigenvalues are easy to identify.

### Symmetries and Commutation

An operator's **symmetries** correspond to transformations that leave it unchanged. If a unitary transformation $U_s$ is a symmetry of an operator $\hat{O}$, the transformed operator $\tilde{O}$ is equal to the original:

$$
\tilde{O} = U_s \hat{O} U_s^\dagger = \hat{O}
$$

This implies that $U_s$ **commutes** with $\hat{O}$:

$$
[\hat{O}, U_s] = 0
$$

In the case of the Hamiltonian, the symmetries of the system provide valuable information about its eigenstates. If a symmetry operator commutes with the Hamiltonian, the eigenstates of the symmetry operator must also be eigenstates of the Hamiltonian, assuming the spectrum is non-degenerate.

### Symmetries and the Hamiltonian

Knowing the symmetries of a Hamiltonian gives us insights into its spectrum. For example, the Hamiltonian of a free particle has translational symmetry, meaning that the physics of the system does not change when the particle is displaced. The eigenstates of the free particle Hamiltonian are plane waves, which are also eigenstates of momentum. This symmetry reflects the fact that momentum commutes with the free particle Hamiltonian. The underlying translational symmetry ensures that the wave function's probability distribution remains the same everywhere.
