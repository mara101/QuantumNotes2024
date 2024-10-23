
In quantum mechanics, when an operator acts on a quantum state and the result is proportional to the original state, the state is called an **eigenstate** (or **eigenfunction** if the state is a function), and the proportionality constant is called the **eigenvalue**.
## Definitions

1. **Eigenvalue**: 
   The **eigenvalue** is the constant $a$ in the equation:
   $$
   \hat{A} |\psi\rangle = a |\psi\rangle
   $$
   where:
   - $\hat{A}$ is a linear operator (such as the Hamiltonian $\hat{H}$),
   - $|\psi\rangle$ is a vector in the Hilbert space (or wavefunction if in function space),
   - $a$ is the **eigenvalue**, which represents a measurable quantity in quantum mechanics (e.g., energy).

2. **Eigenfunction**:
   In cases where the vectors are functions (such as wavefunctions in quantum mechanics), the state $|\psi\rangle$ is referred to as an **eigenfunction**. The equation becomes:
   $$
   \hat{A} \psi(x) = a \psi(x)
   $$
   where $\psi(x)$ is the eigenfunction, and $a$ is its corresponding eigenvalue.

## Key Concepts

1. **Operators in Quantum Mechanics**:
   - Quantum mechanical operators (such as the Hamiltonian $\hat{H}$) often have a set of eigenfunctions and corresponding eigenvalues.
   - For example, if $\hat{H}$ represents the energy of the system, then the eigenvalue $E$ represents the energy associated with the eigenfunction (the wavefunction of the system in that energy state).

2. **Eigenvalue Equation**:
   The general form of the eigenvalue equation is:
   $$
   \hat{A} |\psi\rangle = a |\psi\rangle
   $$
   The operator $\hat{A}$ acting on the state $|\psi\rangle$ results in the same state multiplied by the eigenvalue $a$. This is a characteristic equation that defines the eigenstate and the corresponding measurable quantity (the eigenvalue).

3. **Discrete vs. Continuous Eigenvalues**:
   - In some systems, the eigenvalues are **discrete**, meaning there are specific, distinct values for the measured quantity (e.g., the energy levels of an electron in a hydrogen atom).
   - In other systems, the eigenvalues are **continuous**, meaning the measurable quantity can take any value within a range (e.g., the position of a free particle).

4. **Physical Interpretation**:
   In quantum mechanics, eigenvalues correspond to the possible results of measuring a physical observable (like energy, position, momentum, etc.). The eigenfunction (or eigenstate) is the state of the system immediately after the measurement, with the measured value being the corresponding eigenvalue.

## Example: Hamiltonian Operator

In quantum mechanics, the **Hamiltonian operator** $\hat{H}$ represents the total energy of the system. The eigenvalue equation for the Hamiltonian is:

$$
\hat{H} \psi(x) = E \psi(x)
$$

where:
- $\hat{H}$ is the Hamiltonian,
- $\psi(x)$ is the eigenfunction (the wavefunction of the system in a specific energy state),
- $E$ is the eigenvalue, which represents the **energy** of the system.

## Properties of Eigenvalues and Eigenfunctions

1. **Real Eigenvalues for Hermitian Operators**:
   - In quantum mechanics, operators corresponding to observables (e.g., $\hat{H}$ for energy, $\hat{x}$ for position) are **Hermitian**. Hermitian operators always have **real** eigenvalues, which is important because measurable physical quantities must be real numbers.

2. **Orthogonality of Eigenfunctions**:
   - Eigenfunctions corresponding to **different eigenvalues** of a Hermitian operator are **orthogonal**. This means if $|\psi_1\rangle$ and $|\psi_2\rangle$ are eigenfunctions with different eigenvalues, then:
   $$
   \langle \psi_1 | \psi_2 \rangle = 0
   $$
   - Orthogonality allows for the construction of an orthonormal basis in the Hilbert space, simplifying the analysis of quantum systems.

3. **Degeneracy**:
   - Sometimes, multiple eigenfunctions correspond to the same eigenvalue. This is known as **degeneracy**. For example, in the [[HYDROGEN ATOM|hydrogen atom]], different quantum states can share the same energy eigenvalue.

