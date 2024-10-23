
In quantum mechanics, the free particle problem is an important example used to explore the implications of the wave function. A **free particle** is one that moves in space without any external potential acting on it, i.e., the potential energy $V(x) = 0$ everywhere. While simple in classical mechanics, this scenario reveals deeper wave-like properties in quantum mechanics.
## Time-Independent Schrödinger Equation

The time-independent Schrödinger equation for a free particle is(considering a null energy potential):

$$
-\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} = E \psi(x)
$$

This simplifies to:

$$
\frac{d^2 \psi(x)}{dx^2} = -k^2 \psi(x)
$$

where $k = \sqrt{\frac{2mE}{\hbar^2}}$. For reasons that will be clearer later we express the solution as a sum of exponential and not as we have seen in the case of the [[THE INFINITE SQUARE WELL|the infinite square well]]. The general solution to this differential equation is:

$$
\psi(x) = Ae^{ikx} + Be^{-ikx}
$$

This solution represents a superposition of two plane waves: one moving to the right ($Ae^{ikx}$) and the other to the left ($Be^{-ikx}$).

## Time-Dependent Wave Function

The time-dependent wave function can be obtained by adding the time evolution factor $e^{-iEt/\hbar}$, which leads to the full time-dependent solution:

$$
\psi(x, t) = Ae^{i(kx - \frac{\hbar k^2}{2m}t)} + Be^{-i(kx + \frac{\hbar k^2}{2m}t)}
$$

This describes wave-like motion of the free particle, evolving over time.

## Energy and Momentum

The total energy of a free particle is purely kinetic:

$$
E = \frac{p^2}{2m} = \frac{\hbar^2 k^2}{2m}
$$

Using the de Broglie relation, the momentum of the particle is related to the wave number $k$ by:

$$
p = \hbar k
$$

Thus, the energy and momentum are directly related to the wave number $k$, consistent with the wave-particle duality.

## Group and Phase Velocity

A key aspect of wave mechanics is the distinction between **phase velocity** and **group velocity**. Both are important for understanding how wave packets evolve and propagate.

1. **Phase Velocity**: This is the speed at which the individual wave crests move. It is given by the ratio of the angular frequency $\omega$ to the wave number $k$:

   $$
   v_{\text{phase}} = \frac{\omega}{k}
   $$

   For a free particle, using the dispersion relation $\omega = \frac{\hbar k^2}{2m}$, the phase velocity is:

   $$
   v_{\text{phase}} = \frac{\hbar k}{2m}
   $$

   The phase velocity depends on the wave number $k$. Physically, this represents the speed at which a single monochromatic component of the wave function moves.

2. **Group Velocity**: The group velocity is the speed at which the overall wave packet (which represents a localized particle) moves. It is calculated as the derivative of the angular frequency $\omega$ with respect to the wave number $k$:

   $$
   v_{\text{group}} = \frac{d\omega}{dk} = \frac{\hbar k}{m}
   $$

   This is the velocity of the wave packet, which corresponds to the classical velocity of the particle. For a free particle, the group velocity is exactly twice the phase velocity:

   $$
   v_{\text{group}} = 2v_{\text{phase}}
   $$

   This relationship highlights an important point: the **phase velocity** is slower than the **group velocity**, which is the velocity that corresponds to the actual movement of the particle in a classical sense. The group velocity is associated with the particle's kinetic energy and momentum, while the phase velocity reflects the motion of the wave's crests.

## Non-normalizability and Wave Packets

One complication of the free particle scenario is that plane wave solutions like $\psi(x) = Ae^{ikx} + Be^{-ikx}$ are **non-normalizable**. The integral of $|\psi(x)|^2$ over all space diverges, meaning that these solutions cannot represent a physical particle that is localized in space.

To resolve this, we use **wave packets**, which are a superposition of plane waves with different wave numbers. A wave packet is represented as:

$$
\psi(x, t) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \phi(k) e^{i(kx - \frac{\hbar k^2}{2m}t)} dk
$$

Here, $\phi(k)$ is a function that describes the distribution of wave numbers (or momenta). A wave packet can represent a particle that is localized in space at a given time and moves with the group velocity.
Now if we want to find the solutions of that equations we have also to find $\phi(k)$. For that purpose we use the [[LINKS BETWEEN FOURIER SERIES AND THE SCHRODINGER EQUATION|the Fourier transform]].

![[Screenshot_20241006_154610.png]]