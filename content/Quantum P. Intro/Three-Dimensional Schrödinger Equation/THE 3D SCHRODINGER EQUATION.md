
In this note, we extend our understanding of quantum mechanics to the three-dimensional case. Our goal is to predict the time evolution of a quantum system's state $|\Psi(t)\rangle$ based on its initial condition $|\Psi(0)\rangle$ and the Hamiltonian governing its dynamics. The interesting aspect from a quantum information perspective is that the system’s initial state, which can be a superposition of potentially infinite quantum states (the eigenstates of the Hamiltonian), evolves simultaneously across all these states. Specifically, the quantum state at time $t$ is expressed as:

$$
|\Psi(t)\rangle = \sum_E e^{-i \frac{E}{\hbar} t} c_E |\psi_E\rangle \equiv e^{-i \frac{H}{\hbar} t} \sum_E c_E |\psi_E\rangle = e^{-i \frac{H}{\hbar} t} |\Psi(0)\rangle
$$

This shows that through the appropriate engineering of the Hamiltonian $H$, all energy eigenstates $|\psi_E\rangle$ transform simultaneously in a controlled manner, theoretically allowing for an infinite number of operations to be performed at once.
## The 3D Schrödinger Equation

We now introduce the $x$, $y$, and $z$ coordinates for a particle, along with the corresponding momentum components $p_x$, $p_y$, and $p_z$. The **commutation relations** of these variables extend naturally from the one-dimensional case. The spatial coordinates of a particle can be measured simultaneously because their commutators vanish:

$$
[x, y] = 0 = [x, z] = [y, z]
$$

Similarly, the momentum components commute with each other:

$$
[p_\alpha, p_\beta] = 0 \quad \text{for} \quad \alpha, \beta = x, y, z
$$

However, measuring a position component affects the same component of momentum, leading to the familiar commutation relation between position and momentum:

$$
[\alpha, p_\beta] = \delta_{\alpha\beta} i \hbar \quad \text{for} \quad \alpha, \beta = x, y, z
$$

The representation of position and momentum in configuration space follows the same principles as in one dimension. Specifically:

$$
\hat{r} \to x \hat{u}_x + y \hat{u}_y + z \hat{u}_z
$$
$$
\hat{p} \to -i \hbar (\hat{u}_x \partial_x + \hat{u}_y \partial_y + \hat{u}_z \partial_z) \equiv -i \hbar \nabla_r
$$

Thus, the **Hamiltonian** for a single particle in 3D becomes:

$$
\hat{H} = -\frac{\hbar^2}{2m} \nabla_r^2 + U(r)
$$

where $\nabla_r^2 = \partial_x^2 + \partial_y^2 + \partial_z^2 \equiv \Delta_r$, also known as the **Laplacian**.

### Solutions to the 3D Schrödinger Equation

For specific potentials, one can find **eigensolutions** $\psi_E(r)$ of the Hamiltonian. Consider the case of a **free particle**. The eigenvalue equation reads:

$$
-\frac{\hbar^2}{2m} \nabla_r^2 \psi(r) = E \psi(r)
$$

We can search for a solution in a **separable form**:

$$
\psi(r) = \psi(x) \psi(y) \psi(z)
$$

Inserting this into the eigenvalue equation and separating variables, we obtain three independent equations, each depending only on one spatial coordinate. Each term contributes a constant:

$$
E_\alpha = \frac{\hbar^2 k_\alpha^2}{2m} \quad \text{for} \quad \alpha = x, y, z
$$

Summing these terms gives the total energy $E$, and the wave function $\psi(r)$ becomes:

$$
\psi(r) = e^{i \mathbf{k} \cdot \mathbf{r}}
$$

where $E = \frac{\hbar^2 k^2}{2m}$ and $k = \sum_\alpha k_\alpha \hat{u}_\alpha$.

### Degeneracy in 3D Systems

In more than one dimension, multiple wave vectors $\mathbf{k}$ can have the same magnitude, leading to **degeneracy**. This is especially pronounced in systems with rotational symmetry. For example, in 3D, the energy depends only on the magnitude of $k$, not its direction, leading to a **degeneracy** corresponding to the surface of a sphere in $k$-space.

### 3D Harmonic Oscillator

Consider the 3D [[HARMONIC OSCILLATOR|harmonic oscillator]] with potential energy:

$$
U(r) = \frac{1}{2} m \omega^2 r^2
$$

The eigenvalue equation is separable in this case as well, with the solution written as a product of one-dimensional eigensolutions. The energy for the harmonic oscillator is:

$$
E_{\text{HO}} = \hbar \omega \left( n_x + n_y + n_z + \frac{3}{2} \right)
$$

This system exhibits degeneracy, with the same energy corresponding to different combinations of $n_x$, $n_y$, and $n_z$.

