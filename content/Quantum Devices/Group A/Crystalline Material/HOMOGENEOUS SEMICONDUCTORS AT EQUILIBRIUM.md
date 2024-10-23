
In homogeneous semiconductors at thermal equilibrium, the key consideration is that the system is spatially invariant, with both electron and hole concentrations and the [[DOPING CHEMICAL INTERPRETATION|dopant]] concentrations remaining uniform throughout the material. In this case, there is no external influence such as an electric field or temperature gradient, ensuring a stable environment where the system reaches a steady state.

In such a scenario, both donor ($N_D$) and acceptor ($N_A$) atoms are uniformly distributed, and their concentrations remain spatially constant. For silicon, the typical doping concentrations are within the range of $10^{14} \, \text{cm}^{-3}$ to $10^{20} \, \text{cm}^{-3}$. At thermal equilibrium, part of the donor and acceptor atoms become ionized, contributing to the generation of free charge carriers in the semiconductor.

### Ionized Donor and Acceptor Concentrations
The concentration of ionized donors $N_D^+$ and acceptors $N_A^-$ is influenced by the Fermi level $E_F$. The expressions for these concentrations are given by:

$$
N_D^+ = \frac{N_D}{1 + g_D \exp\left(\frac{E_F - E_D}{k_B T}\right)}
$$

$$
N_A^- = \frac{N_A}{1 + g_A \exp\left(\frac{E_A - E_F}{k_B T}\right)}
$$

Where $E_D$ and $E_A$ are the donor and acceptor energy levels, $g_D$ and $g_A$ are the degeneracy factors, $k_B$ is the Boltzmann constant, and $T$ is the temperature. These relations describe how the ionization of dopants depends on the position of the Fermi level in the energy band structure.

### Local Neutrality Condition
In a homogeneous semiconductor at equilibrium, the system must satisfy local charge neutrality, which ensures that the net charge density in any point of the semiconductor is zero. This condition is expressed as:

$$
q(p - n + N_D^+ - N_A^-) = 0
$$

Here, $n$ is the electron concentration, $p$ is the hole concentration, and $q$ is the elementary charge. This equation reflects the balance between positive and negative charges, including free carriers (electrons and holes) and ionized dopants. At equilibrium, the Fermi level $E_F$ plays a central role in determining the concentrations of free carriers and ionized dopants, ensuring that the charge neutrality condition is satisfied.

### Fermi Level and Free Carrier Concentrations
The relationship between the Fermi level and the free carrier concentrations is described by the Boltzmann approximations, which apply to non-degenerate semiconductors. These approximations state that the electron and hole concentrations are exponentially dependent on the difference between the Fermi level and the conduction or valence band edges:

$$
n = N_c \exp\left(\frac{E_F - E_c}{k_B T}\right)
$$

$$
p = N_v \exp\left(\frac{E_v - E_F}{k_B T}\right)
$$

Where $N_c$ and $N_v$ are the effective densities of states in the conduction and valence bands, respectively, and $E_c$ and $E_v$ are the conduction and valence band edge energies.

