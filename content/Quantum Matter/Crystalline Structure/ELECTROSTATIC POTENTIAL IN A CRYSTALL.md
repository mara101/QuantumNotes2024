
#### Periodicity of the Electrostatic Potential

In a crystal, the electrostatic potential is periodic due to the regular, repeating arrangement of atoms. This periodicity can be mathematically expressed as:

$$V(\vec{r}) = V(\vec{r} + \vec{R}_n)$$

where $\vec{R}_n$ is a lattice translation vector, indicating that the potential at any point $\vec{r}$ is the same as the potential at a corresponding point translated by any lattice vector. This relation is important in understanding how the crystal’s symmetry affects physical properties like the potential field or electronic band structure

#### Fourier Expansion of Periodic Functions

Since the electrostatic potential is periodic, it can be transformed into reciprocal space using a [[THE FOURIER SERIES AND TRANSFORM|Fourier series expansion]]. In this context, we replace the potential function $V(\vec{r})$ with a more general function $f(\vec{r})$, which represents any periodic scalar function:

$$f(\vec{r})^{\text{Fourier}} = \sum_{\vec{k}} C_{\vec{k}} e^{i \vec{k} \cdot \vec{r}}$$

Here, $\vec{k}$ represents the wavevector in reciprocal space, and $C_{\vec{k}}$ are the Fourier coefficients. Each term in this sum represents a plane wave with a specific wavevector $\vec{k}$, and the sum extends over all reciprocal lattice vectors.

This expression converts the function from real space, where it depends on the position $\vec{r}$, to reciprocal space, where it is described in terms of the wavevector $\vec{k}$. This is a key step in connecting real-space quantities to reciprocal-space descriptions, which is particularly useful in crystallography and condensed matter physics.

#### Periodicity Condition in Reciprocal Space

Given the periodic nature of the function in real space, the Fourier-transformed function must satisfy a corresponding condition in reciprocal space. Applying the translation symmetry to the function, we get:

$$f(\vec{r}) = f(\vec{r} + \vec{R}_n)$$

Substituting the Fourier expansion into this expression:

$$f(\vec{r}) = \sum_{\vec{k}} C_{\vec{k}} e^{i \vec{k} \cdot (\vec{r} + \vec{R}_n)}$$

This simplifies to:

$$f(\vec{r}) = \sum_{\vec{k}} C_{\vec{k}} e^{i \vec{k} \cdot \vec{r}} e^{i \vec{k} \cdot \vec{R}_n}$$

For the periodicity condition to hold, the term involving $e^{i \vec{k} \cdot \vec{R}_n}$ must equal 1, because the function does not change when translated by a lattice vector. Therefore, we require:

$$e^{i \vec{k} \cdot \vec{R}_n} = 1$$

This leads to the condition:

$$\vec{k} \cdot \vec{R}_n = 2\pi m$$

where $m$ is an integer. This equation shows that the allowed wavevectors $\vec{k}$ must satisfy this relationship, which defines the **reciprocal lattice vectors**. These vectors are denoted as $\vec{G}$, so we conclude that:

$$\vec{k} = \vec{G}$$

#### Significance of the Reciprocal Lattice

The result $\vec{k} = \vec{G}$ signifies that the wavevectors allowed in the Fourier expansion are restricted to reciprocal lattice vectors. This is a direct consequence of the periodicity of the potential in the crystal. In other words, the Fourier components of any periodic function in a crystal are characterized by the reciprocal lattice vectors.
