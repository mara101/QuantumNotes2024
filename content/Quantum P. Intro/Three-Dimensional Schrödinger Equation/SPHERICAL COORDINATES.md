### Spherical Coordinates in Quantum Mechanics

In quantum mechanics, especially in problems involving rotational symmetry, **spherical coordinates** are often the most convenient system to use. They simplify the treatment of systems such as atoms, where rotational symmetry plays a key role. Spherical coordinates express the position of a particle in terms of three variables: the **radial distance** $r$, the **polar angle** $\theta$, and the **azimuthal angle** $\varphi$. These coordinates are particularly useful when the system's energy is independent of the direction of the position vector.
#### Definitions

The position of a point in 3D space is given in spherical coordinates by:

- **Radial distance** ($r$): The distance from the origin to the point.
- **Polar angle** ($\theta$): The angle between the position vector and the $z$-axis, often called the "colatitude" or "zenith" angle.
- **Azimuthal angle** ($\varphi$): The angle between the projection of the position vector onto the $xy$-plane and the $x$-axis, often called the "longitude" angle.

These coordinates are related to the Cartesian coordinates $(x, y, z)$ through the following transformations:

$$
x = r \sin\theta \cos\varphi
$$
$$
y = r \sin\theta \sin\varphi
$$
$$
z = r \cos\theta
$$
![[Screenshot_20241023_220536.png]]
#### Volume Element

In spherical coordinates, the volume element (used for integrals over space) is different from that in Cartesian coordinates. It is given by:

$$
dV = r^2 \sin\theta \, dr \, d\theta \, d\varphi
$$

This expression accounts for the spherical geometry and is essential when integrating over spherical regions or when solving the Schrödinger equation in 3D.

#### The Laplacian in Spherical Coordinates

The **Laplacian** operator, which is used in the Schrödinger equation, also takes a more complex form in spherical coordinates. The Laplacian in spherical coordinates is:

$$
\nabla^2 = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \right) + \frac{1}{r^2 \sin\theta} \frac{\partial}{\partial \theta} \left( \sin\theta \frac{\partial}{\partial \theta} \right) + \frac{1}{r^2 \sin^2\theta} \frac{\partial^2}{\partial \varphi^2}
$$

This form of the Laplacian is essential when solving for the wavefunctions in systems with spherical symmetry, such as the hydrogen atom.

