In quantum mechanics, particles exhibit different types of motion depending on their interaction with potential energy barriers. These motions fall into two broad categories: **bound states** and **scattering states**. Understanding the distinctions between these states is essential for solving the [[STATIONARY SOLUTIONS AND TIME INDEPENDENT SCHRODINGER EQUATION|Time independent Schrodinger equation]] in various physical systems.

## Bound States and Scattering States: General Overview

The key difference between bound states and scattering states lies in the particle's confinement. In **bound states**, the particle is trapped within a finite region of space due to the presence of a potential well or an attractive force. In contrast, in **scattering states**, the particle moves freely or interacts weakly with a potential, allowing it to escape to infinity or move across a large spatial region.

### Bound States

Bound states are characterized by discrete energy levels. The energy of a particle in a bound state is typically negative, which reflects that the particle is confined by a potential well.The **total energy** of a particle in a bound state is the sum of its **kinetic energy** and **potential energy**. The potential energy is often chosen to be zero at a reference point, usually at infinity, where the particle is considered free from the potential. This means that within the potential well, the particle's potential energy is negative, as the well is typically modeled as an attractive force.

For a bound state to exist, the particle must have insufficient energy to escape the potential well, meaning that its **total energy** must be less than the energy required to be free of the potential (which is zero at infinity). Therefore, in a bound state, the particle’s **total energy** is negative, indicating that it is trapped within the well and would require additional energy to escape. To escape this potential, the particle would need additional energy. For example, the [[THE INFINITE SQUARE WELL|infinite potential well]] and the [[HARMONIC OSCILLATOR|harmonic oscillator]].

In these cases, the wave function of the particle decays exponentially at large distances. This exponential decay ensures that the probability of finding the particle far from the potential well is zero. Mathematically, bound states are represented by normalizable wave functions. The Schrödinger equation for such systems yields solutions where the wave functions vanish at large distances, indicating that the particle remains confined within the potential well.

### Scattering States

In scattering states, the particle has positive energy, which allows it to move freely over an extended region of space or escape from the potential well altogether. Unlike bound states, the energy spectrum in scattering states is continuous. The wave function in scattering states typically exhibits an oscillatory behavior, often resembling a plane wave or a superposition of plane waves. 

The particle is not confined to any specific region and has a finite probability of being found far from the potential region. These states describe situations where a particle interacts weakly with a potential or moves freely, such as a free particle traveling in space without significant constraints.
## Analysis of Bound and Scattering States Using the Schrödinger Equation

To better understand bound and scattering states, we analyze the energy eigenfunctions and eigenvalues of a single particle under various potential scenarios. Regardless of the specific form of the potential $U(x)$, the Schrödinger equation can be written in the general form (watch the [[THE INFINITE SQUARE WELL|infinite potential well for clarification]]):

$$
\frac{d^2 \psi_E(x)}{dx^2} = -k^2 \psi_E(x),
$$

where $k^2 = \frac{2m(E - U(x))}{\hbar^2}$. The behavior of the wave function depends on the sign of $k^2$, which, in turn, depends on the difference between the particle's total energy $E$ and the potential energy $U(x)$.

### Allowed and Forbidden Regions

Depending on whether the particle's energy $E$ is greater or smaller than the potential $U(x)$, two distinct types of behavior emerge:

- **Allowed Region** ($E \geq U(x)$): In regions where the particle’s total energy $E$ is greater than the potential $U(x)$, $k^2$ is positive. In this case, the general solution to the Schrödinger equation is an oscillatory function, typically represented as a superposition of sine and cosine functions or as complex exponentials (plane waves):
  
  $$
  \psi_E(x) = A \sin(kx) + B \cos(kx),
  $$
  
  where $A$ and $B$ are constants determined by boundary conditions. The particle has positive kinetic energy in these regions, and its wave function exhibits oscillatory behavior.

- **Forbidden Region** ($E < U(x)$): When the particle’s energy is less than the potential energy ($E < U(x)$), $k^2$ becomes negative, implying $k = i\kappa$, where $\kappa$ is real and positive. The Schrödinger equation then becomes:

  $$
  \frac{d^2 \psi_E(x)}{dx^2} = \kappa^2 \psi_E(x).
  $$

  The solutions to this equation are no longer oscillatory but instead take the form of exponential functions:

  $$
  \psi_E(x) = C e^{\kappa x} + D e^{-\kappa x}.
  $$

  These represent exponentially growing and decaying wave functions. In physical situations, only the exponentially decaying solution ($D e^{-\kappa x}$) is acceptable in regions far from the potential well, as the exponentially growing solution ($C e^{\kappa x}$) would lead to a non-normalizable wave function (i.e., infinite probability at large distances).

## Example: The Finite Potential Well
![[Screenshot_20241017_112625.png]]

The diagram illustrates a **finite potential barrier** (rectangular potential barrier), where a particle with energy $E$ is incident from the left, interacts with the potential barrier, and some of the wave is transmitted while some is reflected. This setup demonstrates the **quantum mechanical tunneling effect**.
### Potential Regions in the Finite Well

1. **Region I: $x < 0$ (Incident and Reflected Waves)**  
   In this region, the particle is incident on the potential barrier from the left with energy $E$, which is less than the potential height $U_0$. The potential $U(x) = 0$ in this region. This is the **classically allowed region** for the particle, as its total energy $E$ is greater than the potential energy.

2. **Region II: $0 \leq x \leq L$ (Inside the Barrier)**  
   This is the **potential barrier** region where $U(x) = U_0$, and the potential energy is greater than the particle's energy ($E < U_0$). This creates a **classically forbidden region**, where classically a particle cannot enter. However, quantum mechanically, the wave function penetrates this barrier with an exponentially decaying form. The wave function here is a linear combination of exponential functions.

3. **Region III: $x > L$ (Transmitted Wave)**  
   After interacting with the barrier, some portion of the wave is transmitted to Region III. Here, like Region I, $U(x) = 0$, and the particle continues to move as a plane wave. The **transmitted wave** in this region indicates that the particle has tunneled through the barrier.

### The Schrödinger Equation and Solutions in Each Region

In each region, the behavior of the wave function $\psi(x)$ is determined by solving the Schrödinger equation.

#### Region I: $x < 0$ (Incident and Reflected Waves)

In this region, the potential $U(x) = 0$, so the Schrödinger equation simplifies to:

$$
\frac{d^2 \psi(x)}{dx^2} + k^2 \psi(x) = 0, \quad \text{where} \quad k = \frac{\sqrt{2mE}}{\hbar}
$$

The general solution in Region I is a superposition of an **incident** and a **reflected** wave:

$$
\psi_I(x) = A e^{ikx} + B e^{-ikx}
$$

- $A$: amplitude of the incident wave
- $B$: amplitude of the reflected wave

#### Region II: $0 \leq x \leq L$ (Inside the Barrier)

In this region, the potential is constant and equal to $U_0$, so the Schrödinger equation becomes:

$$
\frac{d^2 \psi(x)}{dx^2} - \kappa^2 \psi(x) = 0, \quad \text{where} \quad \kappa = \frac{\sqrt{2m(U_0 - E)}}{\hbar}
$$

Since $E < U_0$, $\kappa$ is real and positive, and the general solution is a combination of exponentially decaying and growing functions:

$$
\psi_{II}(x) = C e^{\kappa x} + D e^{-\kappa x}
$$

In physical situations, only the exponentially decaying solution ($D e^{-\kappa x}$) is valid at large distances, as the exponentially growing solution would lead to a non-normalizable wave function.

#### Region III: $x > L$ (Transmitted Wave)

Here again, the potential is zero, so the Schrödinger equation takes the same form as in Region I:

$$
\frac{d^2 \psi(x)}{dx^2} + k^2 \psi(x) = 0
$$

The solution is a transmitted wave:

$$
\psi_{III}(x) = F e^{ikx}
$$

- $F$: amplitude of the transmitted wave

#### Continuity Conditions

To determine the reflection and transmission probabilities, we apply the **continuity conditions** at the boundaries $x = 0$ and $x = L$. Both the wave function $\psi(x)$ and its first derivative $\frac{d\psi(x)}{dx}$ must be continuous at these boundaries:

- Continuity at $x = 0$: 
  $$
  \psi_I(0) = \psi_{II}(0), \quad \frac{d\psi_I}{dx}\Big|_{x=0} = \frac{d\psi_{II}}{dx}\Big|_{x=0}
  $$
  
- Continuity at $x = L$: 
  $$
  \psi_{II}(L) = \psi_{III}(L), \quad \frac{d\psi_{II}}{dx}\Big|_{x=L} = \frac{d\psi_{III}}{dx}\Big|_{x=L}
  $$

These conditions allow us to match the coefficients $A$, $B$, $C$, $D$, and $F$, and compute the **transmission coefficient** $T$, which gives the probability of the particle tunneling through the barrier.

## Quantum Tunneling and Transmission Coefficient

The phenomenon where a particle has a finite probability to be found on the other side of the barrier (Region III) even though its energy is less than the height of the barrier is called **quantum tunneling**.

The **transmission coefficient** $T$, which represents the probability of the particle tunneling through the barrier, is given by:

$$
T = \frac{|F|^2}{|A|^2}
$$

This coefficient depends on the barrier width $L$, the particle's energy $E$, and the barrier height $U_0$. As the barrier becomes wider or the difference $U_0 - E$ increases, the transmission coefficient decreases exponentially, making tunneling less likely.

## Discrete vs. Continuous Spectra

As seen in the finite potential well example, bound states are associated with **discrete energy levels**. The particle is confined within a potential, and the energy spectrum is discrete because only specific energy values lead to wave functions that meet the boundary conditions. 

On the other hand, **scattering states** exhibit a **continuous energy spectrum**. In these states, the particle is free to move in regions where the potential is either absent or weak, and it is not confined. Since the particle can have any energy above the potential, the energy levels are not quantized, leading to a continuous spectrum.

Some quantum systems, such as finite potential wells, can exhibit both bound and scattering states, depending on the energy of the particle. For energies less than the potential outside the well ($E < 0$), the particle is in a bound state, with discrete energy levels. However, for energies greater than the potential ($E > 0$), the particle is in a scattering state, moving freely outside the well, with a continuous spectrum.



