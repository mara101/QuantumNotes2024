
In quantum mechanics, **measurement** is an action that affects the quantum state of the object being observed. When we perform a measurement on a quantum system, the system's state **collapses** into an [[EIGENVALUES AND EIGENFUNCTIONS|eigenstate]] of the observable being measured. This collapse is an inherent part of the measurement process, and the corresponding operator is crucial in describing how this transformation occurs.

### Uncertainty and Eigenstates

An important observation is that the **uncertainty** of an observable $\hat{O}$ vanishes only when the system is in one of the observable's eigenstates. This applies to all Hermitian operators, such as position, momentum, or energy. In mathematical terms, given the observable $\hat{O}$ with eigenvalue $\lambda_n$:

$$
\hat{O} | O_n \rangle = \lambda_n | O_n \rangle
$$
Eigenstates
The uncertainty in measuring $\hat{O}$ when the system is in eigenstate $| O_n \rangle$ is zero:

$$
\Delta O = \langle O^2 \rangle_n - \langle O \rangle^2_n = 0
$$

This implies that **eigenvalues** are the only measurable values for any observable. After the measurement, there is no uncertainty, and the system will collapse into the corresponding eigenstate. The experiment will always yield one of the observable’s eigenvalues with high accuracy. Hence, all physical observables in quantum mechanics are represented by **Hermitian operators**, ensuring that the measured values (eigenvalues) are real numbers.

### Projection Operators

When a measurement is made, the system's state collapses into a new state with no uncertainty in the measured observable. This transformation is described by a **projection operator**. For instance, when measuring the momentum of a quantum object, if we measure a value $p$, the state collapses into the eigenstate of momentum $|p\rangle$. The operator that achieves this projection is:

$$
\hat{M}_p = |p\rangle\langle p|
$$

When applied to an arbitrary initial state $|\psi_0\rangle$, the state collapses to the momentum eigenstate:

$$
\hat{M}_p |\psi_0\rangle = \psi_0(p) |p\rangle
$$

where $\psi_0(p) = \langle p | \psi_0 \rangle$ is the complex number representing the projection of the initial state onto the momentum eigenstate.

### General Form of Measurement Operator

In general, we can express any initial state $|\psi_0\rangle$ as a superposition of the eigenstates of an observable $\hat{O}$:

$$
|\psi_0\rangle = \sum_n c_n |O_n\rangle
$$

where $c_n = \langle O_n | \psi_0 \rangle$. If a measurement yields the eigenvalue $\lambda_n$, the system collapses into the corresponding eigenstate $|O_n\rangle$. The **measurement operator** that projects the state onto the eigenstate is:

$$
\hat{M}_{O_n} = |O_n\rangle\langle O_n|
$$

Applying this operator to the initial state yields:

$$
\hat{M}_{O_n} |\psi_0\rangle = c_n |O_n\rangle
$$

### Properties of Projection Operators

One key property of projection operators is **idempotence**, which means applying the operator twice yields the same result as applying it once:

$$
\hat{M}_{O_n}^2 = \hat{M}_{O_n}
$$

This property is a defining characteristic of projection operators, ensuring that once the system is projected onto an eigenstate, subsequent applications of the operator do not change the state. This also means that once the measurement is done, another subsequent measurement will not change the result you once obtained. 

### Probability of Measuring a Specific Eigenvalue

Given the initial state $|\psi_0\rangle$, the **probability** of measuring the eigenvalue $\lambda_n$ for the observable $\hat{O}$ is given by the expectation value of the measurement operator:

$$
\langle \psi_0 | \hat{M}_{O_n} | \psi_0 \rangle = |c_n|^2
$$

This probability corresponds to the square of the projection of the initial state onto the eigenstate $|O_n\rangle$.

### Uncertainty Principle and Commutators

The **uncertainty principle** can be better understood by analyzing the simultaneous measurement of two observables, $\hat{A}$ and $\hat{B}$. The uncertainty in measuring both observables vanishes if and only if they share at least one common eigenstate. In this case, their commutator acting on this common eigenstate is zero:

$$
[\hat{A}, \hat{B}] |c\rangle = 0
$$

If the commutator of two observables is a constant different from zero, they cannot be measured simultaneously without uncertainty. For instance, if $[\hat{A}, \hat{B}] \neq 0$, then the measurement of $\hat{A}$ collapses the system into an eigenstate of $\hat{A}$, which cannot simultaneously be an eigenstate of $\hat{B}$. As a result, the measurement of $\hat{B}$ will exhibit non-zero uncertainty, being a superposition of its eigenstates with different eigenvalues.

