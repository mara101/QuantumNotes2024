
Recalling the definition of the density of states $D(E)$, we can start by sketching a simplified plot of the density of states as a function of energy, $D(E)$, and the probability of electron occupation. In this plot:
- On the left, we have $D(E)$, which describes how many states are available at each energy level.
- On the right, we have the probability of occupation, $f(E)$, which follows the Fermi-Dirac distribution.
![[Screenshot_20241016_130010.png]]
At absolute zero temperature $(T = 0K)$, all states below the Fermi energy $E_F$ are fully occupied (probability = 1), while those above it are empty (probability = 0). This means that the **valence band** will be completely filled, and the **conduction band** will remain entirely empty.

### Thermal Excitation of Electrons

At temperatures greater than $0K$, the situation changes. Thermal energy excites some electrons (represented in yellow) from the valence band into the conduction band. This thermal excitation allows the material to exhibit conduction properties.

However, the behavior of these electrons is not the same as that of free electrons in a vacuum. They interact with the crystal lattice, which affects their motion. As a result, their effective mass is different from that of a free electron. Understanding this **effective mass** is crucial to explaining how electrons move in a crystal and their role in the material's electrical properties.

### Free Particle Mass vs. Effective Mass

For a free electron in a vacuum, the relationship between its mass $m$, energy $E$, and momentum $p$ is straightforward. The kinetic energy of a free particle is given by:

$$
E = \frac{p^2}{2m}
$$

From this, the mass can be expressed as:

$$
m = \frac{p^2}{2E} = \frac{\hbar^{2}k^{2}}{2E}
$$

where $\hbar$ is the reduced Planck’s constant and $k$ is the wavevector.

However, inside a crystal, the electron's motion is influenced by the periodic potential of the lattice, and the simple relationship between energy and momentum no longer holds. This leads to a more complex expression for the electron’s behavior, as the energy $E$ now depends on the wavevector $k$ in a non-linear fashion.
![[Screenshot_20241016_130338.png]]

In this band structure diagram, each $k$ value corresponds to a different energy $E$ and effective mass $m^*$. The curvature of the energy band near a particular $k$-point determines how the electron responds to external forces like electric fields.

### Definition of Effective Mass

To describe the electron's motion inside a crystal in a way that is comparable to free particles, we introduce the concept of **effective mass**. The effective mass quantifies how the electron "feels" the crystal's potential and is defined as:

$$
m^{*}_{ij} = \frac{\hbar^{2}}{\left[ \frac{\partial^{2} E}{\partial k_{i} \partial k_{j}}\right]}
$$

In this expression:
- $m^*_{ij}$ is the effective mass tensor, which can vary based on the directions $i$ and $j$,
- The second derivative of energy with respect to the wavevector $k$ determines the curvature of the energy band.

When the band has a high curvature (i.e., $\frac{\partial^2 E}{\partial k^2}$ is large), the effective mass is small, meaning the electron behaves more like a free particle. Conversely, when the band is flat (low curvature), the effective mass is large, meaning the electron moves sluggishly and responds weakly to external forces.
![[Screenshot_20241016_130825.png|400]]
When the electron has a **negative effective mass**, it behaves differently from an electron with a positive mass. Specifically, a negative effective mass implies that the electron accelerates in the opposite direction to the applied force, which is counterintuitive for a normal particle.
Since dealing with particles of negative mass complicates the interpretation, this behavior is instead described using the concept of a **hole**. A hole is treated as a positively charged particle, which behaves in the same way as an electron with a positive mass would but moves in the opposite direction. This simplifies the physical picture, as we can now think of the absence of an electron (i.e., a hole) as a quasiparticle that responds to forces like a positively charged particle, making it easier to analyze charge transport in semiconductors.
### Equation of Motion

With the introduction of the effective mass, the motion of an electron in a crystal can be described similarly to Newton's second law for free particles:

$$
F = m^* a
$$

Here, $F$ is the force applied to the electron, $m^*$ is the effective mass, and $a$ is the resulting acceleration. This form emphasizes that the effective mass directly influences how the electron accelerates in response to an applied force, such as an electric field.

### Physical Interpretation and Band Structure

The effective mass depends strongly on the band structure of the material:
- **Core electrons**, which are tightly bound to the nucleus, have an effective mass approaching infinity $(m^* \to \infty)$ because they do not respond to external forces.
- Electrons near the **valence band edge** or **conduction band edge** have effective masses determined by the curvature of these bands. Typically, **electrons near the conduction band minimum** have a smaller effective mass, making them more mobile.

