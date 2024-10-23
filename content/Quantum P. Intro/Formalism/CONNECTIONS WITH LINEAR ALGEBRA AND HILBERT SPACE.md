## Connections with Linear Algebra

In quantum mechanics, unlike classical physics, we deal primarily with complex-valued functions. This shift is evident from the Schrödinger equation, which involves complex numbers and is fundamental to describing quantum systems. These complex functions are called [[WAVE FUNCTION AND IT'S STATISTICAL REPRESENTATION|wave function]], and they serve as the mathematical representation of a quantum system's state. However, understanding these wave functions is not straightforward without introducing the concept of _operators_.

Now, the operators in quantum mechanics are a key to accessing these probabilities and interpreting physical observables.. These operators are more abstract than the concrete values of classical physics, and they transform the wave function in specific ways that relate to these observables.
![[Screenshot_20241023_191025.png]]
Mathematically, the wave functions behave like vectors in an infinite-dimensional space, often referred to as Hilbert space. This is where quantum mechanics connects to linear algebra. Just as we can represent physical vectors in three-dimensional space with components, wave functions can be thought of as vectors with infinitely many components, corresponding to the values of the function at different points. Operators, which in finite dimensions might be represented as matrices, act on these infinite-dimensional vectors in a similar manner.

To draw an analogy, consider a vector in three-dimensional space. It has three components, and you can represent it as a column matrix. A matrix can act on this vector to transform it into another vector. In quantum mechanics, this same idea applies but extends to an infinite-dimensional space, where operators act on wave functions, transforming them in ways that correspond to physical processes or measurements.

This framework allows us to exploit familiar mathematical techniques from linear algebra, but with the added complexity that we are dealing with infinite dimensions and complex numbers. For instance, just as in three-dimensional space, where we can decompose a vector into components along different axes, in quantum mechanics, we can express a wave function as a sum (or integral) of components in an infinite-dimensional space. This leads to the concept of an orthonormal basis in this space, where each point in space can be associated with a unit vector, and the wave function can be decomposed into a sum of these unit vectors weighted by function values.
![[Screenshot_20241023_190854.png]]
Operators themselves are also represented as infinite-dimensional matrices in this framework. Just as a matrix transforms one vector into another in finite-dimensional linear algebra, in quantum mechanics, an operator transforms one wave function into another. For example, the action of a linear operator T on a function f(x) can be represented as a transformation of the vector components of f. In an N-dimensional case, this would look like a matrix transforming a column vector, but in quantum mechanics, this extends into the infinite-dimensional case.
## Definition of a Hilbert Space

A **Hilbert space** is a complete inner product space that satisfies the following properties:

1. **Vector Space**: It is a set of vectors (like $|\psi\rangle$ and $|\phi\rangle$) that can be added together and multiplied by scalars, just like in conventional vector spaces.

2. **Inner Product**: The space is equipped with an inner product, denoted by $\langle \psi | \phi \rangle$, which is a function that takes two vectors and returns a complex number. The inner product provides a notion of "angle" and "length" in the space, enabling the measurement of distances and projections. The inner product satisfies:
   - $\langle \psi | \psi \rangle \geq 0$, with equality only when $|\psi\rangle = 0$
   - $\langle \psi | \phi \rangle = \overline{\langle \phi | \psi \rangle}$ (conjugate symmetry)

3. **Completeness**: A Hilbert space is **complete**, meaning that any Cauchy sequence of vectors has a limit within the space. This ensures that there are no "gaps" in the space, making it well-suited for rigorous mathematical descriptions of quantum systems. Completeness ensures that the Hilbert space is closed under the operation of taking limits of sequences of vectors. This is important because physical systems are often described using approximations, and we want to ensure that the limits of these approximations still represent valid quantum states.
   In more intuitive terms, completeness means that there are no "gaps" in the Hilbert space. If you take an infinite series of steps that get progressively smaller, the end result (the limit) must still be a valid element (vector) in the Hilbert space. This is crucial for making the space mathematically stable and reliable for representing physical systems.

4. **Norm and Distance**: The inner product defines a norm (or length) of a vector, given by:
   $$
   ||\psi|| = \sqrt{\langle \psi | \psi \rangle}
   $$
   The distance between two vectors can be measured using this norm.

5. **Infinite Dimensionality**: In quantum mechanics, Hilbert spaces are often **infinite-dimensional**, meaning they contain an infinite number of basis vectors. This is necessary to describe systems with a continuous range of states, such as the position of a particle.

# Bra and Ket in Quantum Mechanics

The **bra** and **ket** are essential components of the mathematical framework used to describe quantum states, known as **Dirac notation**. They play a fundamental role in quantum mechanics for representing vectors and their duals in Hilbert space.

## Ket (|ψ⟩)

A **ket** is a vector in a complex Hilbert space, which represents the state of a quantum system. It is denoted as $|\psi\rangle$, where $\psi$ symbolizes the particular state. For example, the quantum state of a particle could be written as $| \psi \rangle$, and this vector contains all the information about the system.

## Bra (⟨ψ|)

A **bra** is the dual of a ket, which corresponds to a row vector in linear algebra, as opposed to the column vector represented by a ket. It is denoted as $\langle \psi |$, and it operates on kets to produce scalar quantities. Mathematically, it is the complex conjugate transpose of the ket.
![[Screenshot_20241004_104655.png]]

## Bra-Ket Notation and Inner Products

An inner product in quantum mechanics is formed by combining a **bra** (the conjugate transpose of a vector, written as $\langle \psi |$) with a **ket** (a vector, written as $|\phi\rangle$). For example, if $|\psi\rangle$ and $|\phi\rangle$ are two quantum states (kets), their inner product is denoted $\langle \psi | \phi \rangle$, which results in a scalar. This scalar often represents important quantities like probability amplitudes, giving us insight into the likelihood of transitioning between two quantum states. If we have a quantum state $|\psi\rangle$, its corresponding bra is written as $\langle \psi |$. The expression $\langle \psi | \phi \rangle$ represents the *overlap* between the states $|\psi\rangle$ and $|\phi\rangle$. This overlap is critical in determining the probability of transitioning from state $|\psi\rangle$ to state $|\phi\rangle$.

### Inner Product in Hilbert Space

In a **Hilbert space**, which is a mathematical structure that describes the state space of quantum systems, the inner product of two functions $f(x)$ and $g(x)$ is defined as:
$$
\langle f | g \rangle = \int_a^b f(x)^* g(x) \, dx
$$
This inner product satisfies several essential properties, including:
- **Conjugate symmetry**: 
$$
\langle g | f \rangle = \langle f | g \rangle^*
$$
- The inner product of a function with itself is always **real and non-negative**:
$$
\langle f | f \rangle = \int_a^b |f(x)|^2 \, dx
$$

### Orthonormality and Completeness

In quantum mechanics, functions (or vectors in a Hilbert space) are **normalized** if their inner product with themselves is 1:
$$
\langle f | f \rangle = 1
$$
Two functions are **orthogonal** if their inner product is zero, indicating that the states are independent:
$$
\langle f | g \rangle = 0
$$
A set of functions $\{f_n(x)\}$ is **orthonormal** if the inner product between any two distinct functions is zero and the inner product of each function with itself is one:
$$
\langle f_m | f_n \rangle = \delta_{mn}
$$
where $\delta_{mn}$ is the Kronecker delta, which equals 1 when $m = n$ and 0 otherwise.

The set of functions is **complete** if any function in the Hilbert space can be written as a linear combination of these basis functions:
$$
f(x) = \sum_{n=1}^{\infty} c_n f_n(x)
$$
where:
$$
c_n = \langle f_n | f \rangle
$$
This property of completeness is fundamental in quantum mechanics, as it allows us to describe any state in the system using a series of basis functions.

### Outer Products and Operators

While the inner product gives a scalar, the **outer product** involves combining a ket $| f \rangle$ and a bra $\langle g |$, resulting in a **matrix**. The outer product $| f \rangle \langle g |$ produces an operator that can act on vectors or other operators in the space. 
#### Test Example:
Given two vectors $| f \rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$ and $| g \rangle = \begin{pmatrix} 0 \\ i \end{pmatrix}$, their inner product is:
$$
\langle f | g \rangle = 1 \cdot 0 + 0 \cdot (-i) = 0
$$
And their outer product $| f \rangle \langle g |$ results in a matrix:
$$
| f \rangle \langle g | = \begin{pmatrix} 1 \\ 0 \end{pmatrix} \begin{pmatrix} 0 & -i \end{pmatrix} = \begin{pmatrix} 0 & -i \\ 0 & 0 \end{pmatrix}
$$

Now, consider the matrix $T = \begin{pmatrix} 1 & 0 \\ -i & i \end{pmatrix}$. This matrix can be written as a **superposition** of outer products of the vectors $| f \rangle$ and $| g \rangle$.

### Operators as Sums of Outer Products

In quantum mechanics, any operator $\hat{O}$ can be represented as a sum of outer products of vectors from a complete orthonormal basis. If $\{|i\rangle\}$ is a complete set of basis vectors, the operator $\hat{O}$ can be expressed as:
$$
\hat{O} = \sum_{i,j} O_{ij} |i\rangle \langle j|
$$
where $O_{ij} = \langle i | \hat{O} | j \rangle$ are the matrix elements of the operator in this basis.

In particular, the **Hamiltonian** $\hat{H}$ of a system, which represents its total energy, can be expressed in an infinite-dimensional basis $\{|x\rangle\}$ as:
$$
\hat{H} = \int dx H(x) |x\rangle \langle x|
$$
This shows how operators, such as the Hamiltonian, act on the state space by summing over the contributions from each basis vector.

### Completeness of Orthonormal Sets

The concept of completeness can also be framed in terms of outer products. A set of vectors $\{|f_n\rangle\}$ is complete if the sum of their outer products equals the identity operator:
$$
\sum_n | f_n \rangle \langle f_n | = I
$$
This identity operator $I$ ensures that any vector in the space can be reconstructed from the basis vectors. 

For example, if $|g\rangle = \sum_n c_n |f_n\rangle$, then the coefficients $c_n$ are simply given by the inner product:
$$
c_n = \langle f_n | g \rangle
$$

In three-dimensional space, the unit vectors $\hat{i}, \hat{j}, \hat{k}$ form a complete orthonormal set, and any vector can be expressed as a combination of these basis vectors. Similarly, in quantum mechanics, any vector can be written as a linear combination of the basis vectors in the Hilbert space.


