## Angular Momentum
In quantum mechanics, rotational symmetry plays a significant role, just as translational symmetry does in 1D. When the energy of a system is independent of the orientation of the position vector $r$, we have rotational symmetry. This symmetry is related to the conservation of **angular momentum**, analogous to how translational symmetry corresponds to momentum conservation.

#### Classical Angular Momentum

In classical mechanics, the angular momentum $L$ for a particle is defined as the cross product of the position vector $r$ and the momentum $p$:
$$
L = r \times p
$$

#### Quantum Angular Momentum Operator

In the quantum mechanical context, we seek the operator associated with the angular momentum observable. Following the same principles used to quantize other observables, we write the angular momentum operator as:
$$
\hat{L} = -i\hbar (r \times \nabla_r)
$$

This operator arises from the cross product of the position vector and the momentum operator, which is proportional to the gradient $\nabla_r$ in configuration space.

#### Commutation Relations of Angular Momentum

A key feature of angular momentum in quantum mechanics is that not all components of the angular momentum can be measured simultaneously. This is a result of the non-commutative nature of the angular momentum components. Expanding the cross product into its components and using the commutation relations for position and momentum, we find:

$$
[L_x, L_y] = i\hbar L_z
$$
$$
[L_y, L_z] = i\hbar L_x
$$
$$
[L_z, L_x] = i\hbar L_y
$$

 As a result, the components of angular momentum $L_x$, $L_y$, and $L_z$ are **incompatible observables**—meaning that they cannot have simultaneous eigenstates.

#### Total Angular Momentum

Although it is impossible to measure all three components of angular momentum at once, the **magnitude** of the angular momentum, denoted $L^2$, commutes with each individual component. Specifically, we have the commutator:

$$
[L^2, L_\alpha] = 0 \quad \text{for} \quad \alpha = x, y, z
$$

This means that while we cannot have a state with definite values for all components of angular momentum, we can have a state with a well-defined total angular momentum $L^2$ and a well-defined component in a chosen direction, usually $L_z$. These two quantities share a common set of **eigenfunctions**, which is particularly useful for solving the time-independent Schrödinger equation when the Hamiltonian is invariant under rotations.

#### Simultaneous Eigenfunctions of $L^2$ and $L_z$

The quantum states of angular momentum are characterized by the simultaneous eigenfunctions of $L^2$ and $L_z$. However, due to the commutation relations, we lose information about the other two components of angular momentum, $L_x$ and $L_y$, which remain indeterminate in such states.

#### Uncertainty Relations for Angular Momentum

The incompatibility of measuring different components of angular momentum simultaneously gives rise to an uncertainty relation, similar to the uncertainty principle for position and momentum. Specifically, for the components $L_x$ and $L_y$, the uncertainty relation is given by:

$$
\Delta L_x \Delta L_y \geq \frac{\hbar}{2} | \langle L_z \rangle |
$$

This relation shows that the uncertainties in $L_x$ and $L_y$ are constrained by the expectation value of $L_z$.

##### Question: When can this uncertainty be zero?
The uncertainty cannot be zero due to the non-commutative nature of the angular momentum components, but in cases where $\langle L_z \rangle = 0$, the uncertainty product will be minimized.

## Magnetic Quantum Number

We have just learned that while not all components of angular momentum can be measured simultaneously, it is possible to measure the **magnitude** of angular momentum, denoted by $L^2$, along with one specific component, typically chosen to be $L_z$. The measurable values of these quantities are their **eigenvalues**.

#### Eigenvalues of $L_z$

Let’s take a closer look at the eigenvalue equation for the $L_z$ operator, which represents the angular momentum component along the $z$-axis, specifically in [[SPHERICAL COORDINATES|spherical coordinates]]. This coordinate system simplifies the problem due to its symmetry and allows for a clearer understanding of how angular momentum behaves in quantum systems.

The eigenvalue equation for $L_z$ is:

$$
L_z \phi_m(\varphi) = \hbar m \phi_m(\varphi)
$$

Here, $\phi_m(\varphi)$ represents the wavefunction that depends on the azimuthal angle $\varphi$, and $m$ is a quantum number that characterizes the angular momentum along the $z$-axis. The key point is that the eigenvalues of $L_z$ are **quantized**—meaning that $L_z$ can only take specific discrete values, which are integer multiples of $\hbar$. These values are given by $\hbar m$, where $m$ is an integer (i.e., $m \in \mathbb{Z}$).

#### The $L_z$ Operator in Spherical Coordinates

In spherical coordinates, the operator for $L_z$ is given by:

$$
L_z = -i\hbar \frac{\partial}{\partial \varphi}
$$

This expression shows that $L_z$ is related to the rate of change of the wavefunction with respect to the azimuthal angle $\varphi$. The factor $-i\hbar$ reflects the fact that angular momentum has the same physical dimensions as Planck’s constant $\hbar$, which quantifies the smallest unit of angular momentum.

#### Solving the Eigenvalue Equation

The eigenvalue equation $L_z \phi_m(\varphi) = \hbar m \phi_m(\varphi)$ can be solved by substituting the form of $L_z$. This leads to the differential equation:

$$
-i\hbar \frac{\partial}{\partial \varphi} \phi_m(\varphi) = \hbar m \phi_m(\varphi)
$$

Dividing both sides by $-i\hbar$, we get:

$$
\frac{\partial}{\partial \varphi} \phi_m(\varphi) = im \phi_m(\varphi)
$$

The general solution to this differential equation is:

$$
\phi_m(\varphi) = C(r, \theta) e^{im\varphi}
$$

where $C(r, \theta)$ is a function of the radial and polar coordinates, and the term $e^{im\varphi}$ describes the azimuthal dependence of the wavefunction. This solution shows that the wavefunction $\phi_m(\varphi)$ varies as a complex exponential with respect to the azimuthal angle $\varphi$.

#### Physical Meaning of Quantization

For this solution to be **physically meaningful**, the wavefunction must be single-valued, meaning that the value of $\phi_m(\varphi)$ must be the same after a complete rotation (i.e., after an increase of $2\pi$ in $\varphi$). This is because the azimuthal angle $\varphi$ represents a periodic coordinate—moving $2\pi$ radians (a full circle) in $\varphi$ brings us back to the same physical point.

To ensure this periodicity, the exponential term $e^{im\varphi}$ must satisfy:

$$
e^{im(\varphi + 2\pi)} = e^{im\varphi}
$$

This condition holds only if $m$ is an integer, as the exponential function of an integer multiple of $2\pi$ equals 1:

$$
e^{im2\pi} = 1 \quad \text{if} \quad m \in \mathbb{Z}
$$

Thus, $m$ must be an integer, which implies that the eigenvalues of $L_z$ are **quantized**. This means that $L_z$ can only take discrete values that are integer multiples of $\hbar$, confirming that angular momentum is fundamentally quantized in quantum mechanics.

#### Magnetic Quantum Number

The integer $m$ is referred to as the **magnetic quantum number**, reflecting its historical association with the behavior of angular momentum in a magnetic field. Importantly, the quantization of $L_z$ implies that angular momentum in a specific direction cannot take arbitrary values; it is constrained to discrete multiples of $\hbar$.

Since the choice of the $z$-axis is arbitrary, this result holds for angular momentum along any direction. Moreover, if the surrounding environment (such as the potential or the Hamiltonian) has **rotational symmetry**, the energy of the system does not depend on the specific value of $m$. This suggests that angular momentum in any arbitrary direction is physically irrelevant to the energy levels of the system, and the Hamiltonian commutes with all components of angular momentum:

$$
[H, L_\alpha] = 0 \quad \text{for} \quad \alpha = x, y, z
$$

Thus, the value of $m$ does not affect the energy eigenvalue, so rotational symmetry implies that energy is independent of the orientation of angular momentum.

#### Canonical Conjugacy and Uncertainty

The angle $\varphi$ and the angular momentum component $L_z$ are **canonically conjugate variables**, analogous to the position and momentum variables in one dimension. This is captured by the commutation relation:

$$
[\varphi, L_z] = i\hbar
$$

This implies that, just like position and momentum, there is an **uncertainty principle** between $\varphi$ and $L_z$. Specifically, reducing the uncertainty in one will increase the uncertainty in the other. If the uncertainty in the azimuthal angle $\varphi$ is minimized (for example, by trying to localize the particle's position on the circle), the uncertainty in $L_z$ will increase.

