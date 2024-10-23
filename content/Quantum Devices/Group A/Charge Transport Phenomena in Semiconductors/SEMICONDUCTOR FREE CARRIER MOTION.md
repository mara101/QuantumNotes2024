## Charge Transport without an electric field
At thermal equilibrium, the current density throughout the semiconductor is zero. This condition does not imply that the free carriers (electrons in the conduction band and holes in the valence band) are stationary. On the contrary, due to thermal energy, these carriers are constantly in motion. What thermal equilibrium implies is that the *net* or *average* current density is zero. This means that while individual carriers are moving, there is no overall drift of charge in any particular direction when averaged over time and space.

In a sufficiently large volume of semiconductor material, there will be a large number of electrons ($N_n = nV$) and holes ($N_p = pV$), where $n$ and $p$ are the volume concentrations of electrons and holes, respectively, and $V$ is the volume. Each of these particles has an instantaneous velocity ($\mathbf{v}_{ni}$ for electrons and $\mathbf{v}_{pi}$ for holes) due to thermal agitation, which means that they are moving randomly and rapidly at any given instant. The thermal velocities are not zero, even though the average velocity (or drift velocity) of the ensemble of particles must be zero to satisfy the zero net current condition.

The drift velocities of electrons ($\mathbf{v}_n$) and holes ($\mathbf{v}_p$) are defined as the average of the individual instantaneous velocities of all the electrons and holes, respectively:

$$
\mathbf{v}_n = \frac{1}{N_n} \sum_{i=1}^{N_n} \mathbf{v}_{ni}
$$

$$
\mathbf{v}_p = \frac{1}{N_p} \sum_{i=1}^{N_p} \mathbf{v}_{pi}
$$

While the average of these velocities is zero at equilibrium (indicating no net current), the root mean square (RMS) value of the instantaneous velocities is not zero. This RMS value gives rise to the thermal velocity ($v_{th}$), which can be calculated using the equipartition theorem from statistical mechanics. For a particle with three degrees of freedom (moving freely in three-dimensional space), the theorem states:

$$
\frac{1}{2} m_n^* v_{th,n}^2 = \frac{3}{2} k_B T
$$

$$
\frac{1}{2} m_p^* v_{th,p}^2 = \frac{3}{2} k_B T
$$

Here, $m_n^*$ and $m_p^*$ are the [[EFFECTIVE MASS(QCMP)]] of the electron and hole, respectively, $k_B$ is Boltzmann's constant, and $T$ is the absolute temperature. From these equations, the thermal velocities of electrons and holes are given by:

$$
v_{th,n} = \sqrt{\frac{3 k_B T}{m_n^*}}
$$

$$
v_{th,p} = \sqrt{\frac{3 k_B T}{m_p^*}}
$$

These thermal velocities are substantial, meaning that even at thermal equilibrium, the carriers are in constant, rapid motion.

The motion of carriers in a perfect crystalline lattice is characterized by periods of "free flight" (where carriers move linearly, either uniformly if there is no electric field, or accelerated if there is an electric field) interrupted by collisions. These collisions can be caused by various factors such as crystal dislocations, impurities, or lattice vibrations ([[PHONONS|phonons]]). The mean time between collisions is called the collision time or mean free time ($\tau_C$), which is also related to the mean distance between collisions, known as the mean free path ($\lambda$).

## Charge Transport in Semiconductors Under an Electric Field

In the presence of an electric field $\mathbf{E}$, free charges in a semiconductor are accelerated according to the force acting on them. The force $\mathbf{F}$ on a charge $Q$ in an electric field is given by:

$$
\mathbf{F} = Q \mathbf{E}
$$

This force accelerates holes, which carry a positive charge $Q = +q$, in the direction of the electric field, while electrons, with negative charge $Q = -q$, are accelerated in the opposite direction. These movements are essential for understanding how current flows in semiconductors.

The dynamics of charge carriers (electrons and holes) follow Newton’s second law, which, in the case of momentum, is expressed as:

$$
\frac{d \mathbf{q}_n}{dt} = -q \mathbf{E} + \text{collisions}
$$

$$
\frac{d \mathbf{q}_p}{dt} = +q \mathbf{E} + \text{collisions}
$$

Here, $\mathbf{q}_n$ and $\mathbf{q}_p$ are the momenta of electrons and holes, respectively. The term "collisions" refers to the effects of scattering events that occur due to impurities, lattice vibrations (phonons), or other charge carriers. These collisions cause changes in the momentum of the particles, acting as a form of resistance to their motion.

### Averaged Motion and Collisions

The average momentum for a large ensemble of particles can be calculated by summing the individual momenta of all carriers. For $N_n$ electrons and $N_p$ holes, the average force due to the electric field is:

$$
\frac{1}{N_n} \sum_{i=1}^{N_n} (-q \mathbf{E}) = -q \mathbf{E}
$$

$$
\frac{1}{N_p} \sum_{i=1}^{N_p} (+q \mathbf{E}) = +q \mathbf{E}
$$

Thus, the evolution equations for the average momenta of electrons and holes become:

$$
\frac{d \langle \mathbf{q}_n \rangle}{dt} = -q \mathbf{E} + \langle \text{collisions} \rangle
$$

$$
\frac{d \langle \mathbf{q}_p \rangle}{dt} = +q \mathbf{E} + \langle \text{collisions} \rangle
$$

Under stationary conditions (where time derivatives of the momenta vanish), these equations simplify to:

$$
0 = -q \mathbf{E} - \frac{\langle \mathbf{q}_n \rangle}{\tau_n}
$$

$$
0 = +q \mathbf{E} - \frac{\langle \mathbf{q}_p \rangle}{\tau_p}
$$

Here, $\tau_n$ and $\tau_p$ are the average relaxation times, which characterize how quickly momentum is lost due to collisions for electrons and holes, respectively.

### Drift Velocity and Mobility

The momentum can be related to the velocity using the definition of average momentum, $\langle \mathbf{q}_n \rangle = m_n^* \mathbf{v}_n$ for electrons and $\langle \mathbf{q}_p \rangle = m_p^* \mathbf{v}_p$ for holes, where $m_n^*$ and $m_p^*$ are the effective masses of electrons and holes. Substituting into the previous stationary equations gives the drift velocities:

$$
\mathbf{v}_n = -\frac{q \tau_n}{m_n^*} \mathbf{E} = -\mu_n \mathbf{E}
$$

$$
\mathbf{v}_p = +\frac{q \tau_p}{m_p^*} \mathbf{E} = +\mu_p \mathbf{E}
$$

Here, $\mu_n = \frac{q \tau_n}{m_n^*}$ and $\mu_p = \frac{q \tau_p}{m_p^*}$ are the mobilities of electrons and holes, respectively. This result shows that the drift velocities are proportional to the electric field, establishing a linear relationship between velocity and field strength, a behavior often referred to as **Ohm's law at the microscopic level**.

### Mobility and Scattering

In semiconductors, several types of scattering mechanisms contribute to the overall resistance experienced by charge carriers. These include:
- **Phonon scattering** (due to lattice vibrations),
- **Impurity scattering** (due to dopants or defects), and
- **Carrier-carrier scattering** (interactions between charge carriers).

The total relaxation time $\tau_{\text{eq}}$ (or total mobility) can be found by summing the contributions from individual scattering processes using Mathiessen’s rule:

$$
\frac{1}{\tau_{\text{eq}}} = \sum_k \frac{1}{\tau_k}
$$

This also applies to mobility, yielding:

$$
\frac{1}{\mu_n} = \sum_k \frac{1}{\mu_{n,k}}
$$

$$
\frac{1}{\mu_p} = \sum_k \frac{1}{\mu_{p,k}}
$$

Where $\mu_{n,k}$ and $\mu_{p,k}$ are the mobilities associated with each specific scattering mechanism.

### High-Field Effects and Velocity Saturation

At high electric fields, the linear relationship between drift velocity and electric field no longer holds. As the energy of the carriers increases due to the strong electric field, additional scattering mechanisms become more effective, leading to a **saturation of drift velocity**. This phenomenon is called **velocity saturation**, where the drift velocity approaches a constant value independent of further increases in the electric field. For most semiconductors, the saturation velocity is approximately $10^7 \, \text{cm/s}$.

Figure 3.1 (referred to in the document) illustrates how the drift velocity depends on the magnitude of the electric field for several semiconductors at room temperature. The initial region shows a linear increase (constant mobility), while at high fields, the velocity saturates.

### Ballistic Transport

In classical devices, the drift velocity is limited by scattering, as described by Ohmic behavior. However, in **quantum devices** or **nanometer-scale devices**, where the dimensions are comparable to or smaller than the **mean free path** (the average distance between scattering events), **ballistic transport** becomes significant. In ballistic transport, charge carriers move across the device without scattering, resulting in much faster response times and improved performance compared to traditional diffusive transport.

### Negative Differential Mobility
![[Screenshot_20241020_120914.png]]

In some materials like GaAs and InP, increasing the electric field can cause a decrease in the electron drift velocity. This phenomenon is known as **negative differential mobility**. It occurs in certain regions of the electric field, where higher fields cause more frequent scattering, reducing the net velocity of carriers. This effect is important in the operation of high-speed and high-frequency electronic devices.
### Influence of Doping and Temperature

Carrier mobility in semiconductors is affected by doping and temperature:
- **Doping** increases impurity scattering. Higher dopant concentrations lead to more frequent collisions with impurity atoms, thereby reducing the mobility of both electrons and holes.
- **Temperature** influences mobility through phonon scattering. As the temperature rises, lattice vibrations increase, leading to more frequent phonon interactions, which reduce mobility.

The mobility’s dependency on temperature follows an approximate relationship:

$$
\mu(T) \propto T^{-\alpha}
$$
![[Screenshot_20241020_121217.png]]
Where $\alpha$ is typically between 2.2 and 2.4 for common semiconductors. Figure 3.3 depicts the experimental temperature dependence of low-field mobility for silicon, showing a clear decrease with increasing temperature.

### Mobility Models

An empirical model often used to describe the mobility’s dependence on total doping concentration $N_t$ is given by:

$$
\mu = \mu_{\text{min}} + \frac{\mu_{\text{max}} - \mu_{\text{min}}}{1 + (N_t / N_{\text{REF}})^\alpha}
$$

Where $\mu_{\text{max}}$, $\mu_{\text{min}}$, $N_{\text{REF}}$, and $\alpha$ are material-specific parameters. This model is used to fit experimental data, such as the mobility curves for electrons and holes in silicon as a function of doping concentration.
![[Screenshot_20241020_121622.png]]
## Diffusion in Semiconductors

Diffusion occurs whenever particles exhibit a spatially non-uniform density. According to thermodynamic principles, particles naturally move from regions of higher concentration to areas with lower concentration, creating a net particle flow or flux. This motion compensates for concentration differences.

The **net particle flux** vector $\mathbf{\Phi}$, representing the number of particles crossing a unit section per unit time, is related to the particle concentration $c$ by **Fick's law**:

$$
\mathbf{\Phi} = -D \nabla c
$$

where $\nabla$ is the gradient operator, and $D$ is the diffusion coefficient or diffusivity of the particles (with units of cm\(^2\)/s).
![[Screenshot_20241020_121851.png]]
### Diffusion in Semiconductors with Charge

In semiconductors, free particles (electrons and holes) carry electric charge. Thus, their diffusion results in a **current density**:

$$
\mathbf{J}_{n,\text{diff}} = -q \mathbf{\Phi}_n = +q D_n \nabla n
$$

$$
\mathbf{J}_{p,\text{diff}} = +q \mathbf{\Phi}_p = -q D_p \nabla p
$$

For one-dimensional diffusion, these equations simplify to:

$$
J_{n,\text{diff}} = +q D_n \frac{\partial n}{\partial x}
$$

$$
J_{p,\text{diff}} = -q D_p \frac{\partial p}{\partial x}
$$

Here, $D_n$ and $D_p$ are the **diffusivities** for electrons and holes, respectively.

### Einstein Relation

At thermodynamic equilibrium, the diffusivity $D$ and mobility $\mu$ of charge carriers are related by the **Einstein relationship**:

$$
D_n = \frac{k_B T}{q} \mu_n = V_T \mu_n
$$

$$
D_p = \frac{k_B T}{q} \mu_p = V_T \mu_p
$$

where $k_B$ is the Boltzmann constant, $T$ is the temperature, $q$ is the elementary charge, and $V_T = \frac{k_B T}{q}$ is the **thermal voltage**, which is approximately 26 mV at room temperature ($T = 300$ K).

Although the Einstein relation strictly applies only at thermal equilibrium, it is often a good approximation even out of equilibrium.

### The Drift-Diffusion Model

The **drift-diffusion model** combines the effects of **drift** (motion due to an electric field) and **diffusion** (motion due to concentration gradients) for both electrons and holes. The total current density for each carrier species is the sum of drift and diffusion components:

$$
J_n = J_{n,\text{drift}} + J_{n,\text{diff}} = q n \mu_n E + q D_n \frac{\partial n}{\partial x}
$$

$$
J_p = J_{p,\text{drift}} + J_{p,\text{diff}} = q p \mu_p E - q D_p \frac{\partial p}{\partial x}
$$

In a semiconductor, neglecting displacement currents (which is valid unless the operating frequency is in the GHz range), the total current is given by:

$$
J(x) = J_n(x) + J_p(x) = J_{n,\text{drift}}(x) + J_{n,\text{diff}}(x) + J_{p,\text{drift}}(x) + J_{p,\text{diff}}(x)
$$

### Equilibrium Conditions

At **thermodynamic equilibrium**, there is no net current flow, implying:

$$
J(x) = 0
$$

This is a result of the **detailed balance principle**, which ensures that the drift and diffusion components cancel each other out:

$$
J_n(x) = J_{n,\text{drift}}(x) + J_{n,\text{diff}}(x) = 0
$$

$$
J_p(x) = J_{p,\text{drift}}(x) + J_{p,\text{diff}}(x) = 0
$$

### Quasi-Fermi Levels

When a semiconductor is not in equilibrium, the **quasi-Fermi levels** for electrons ($E_{F_n}$) and holes ($E_{F_p}$) extend the concept of the equilibrium Fermi level. These levels are used to describe carrier concentrations out of equilibrium:

$$
n = n_i \exp\left(\frac{E_{F_n} - E_F}{k_B T}\right)
$$

$$
p = n_i \exp\left(\frac{E_F - E_{F_p}}{k_B T}\right)
$$

Here, $n_i$ is the intrinsic carrier concentration, and $E_F$ is the equilibrium Fermi level. At equilibrium, $E_{F_n} = E_{F_p} = E_F$.

The total current density for each carrier can be expressed in terms of the gradients of the quasi-Fermi levels:

$$
J_n = n \mu_n \frac{\partial E_{F_n}}{\partial x}
$$

$$
J_p = p \mu_p \frac{\partial E_{F_p}}{\partial x}
$$

Thus, in a material with a non-negligible population of free carriers, **zero current density** implies that the corresponding quasi-Fermi energy is constant.
![[Screenshot_20241020_122254.png]]
The bending of the conduction and valence bands indicates a **non-uniform region**, likely a **semiconductor junction** or **heterostructure** where the energy bands shift due to variations in material properties (e.g., doping). The Fermi level varies slightly across the region, suggesting that the material is not in strict thermal equilibrium.

At thermal equilibrium, the Fermi level is uniform throughout the material, as indicated by:

$$
\frac{\partial E_F}{\partial x} = 0
$$
## Electrochemical Potential, Fermi Energy, and Thermal Equilibrium

The concept of **Fermi energy** is a broad one in physics, not limited to semiconductor band theory. It is closely tied to the **chemical potential** $\mu$ of a system, which represents the work required to add a particle to the system or the work obtained by removing a particle. This work is related to the variation in the system's free (Gibbs) energy $G$ with respect to the particle number $N$:

$$
\mu = \frac{\partial G}{\partial N}
$$

In systems with charged particles (such as electrons), an important contribution to the chemical potential comes from the work required due to electrostatic potential variations. This contribution is $-q\Delta \varphi$, where $q$ is the charge of the particle, and $\Delta \varphi$ is the change in electrostatic potential. When such systems are combined, particles flow from regions of higher chemical potential to regions of lower chemical potential. A particle will only transit from system 1 to system 2 if $\mu_1 > \mu_2$, ensuring the work required to move a particle into system 2 is smaller than the work extracted from system 1.

If $\mu_1 = \mu_2$, no net particle flow occurs, meaning the systems are in equilibrium, and no electrical current flows between them. In equilibrium, the chemical potential is **constant**, and there is no net energy exchange within the system. This situation corresponds to **thermodynamic equilibrium**, where the temperature remains unchanged.

### Metals and Semiconductors at Equilibrium

Metals and semiconductors in equilibrium (or quasi-equilibrium) follow the **Fermi-Dirac distribution**. In these thermodynamic systems, the **chemical potential** corresponds to the **Fermi energy**:

$$
\mu = E_F
$$

This relation holds because in a degenerate electron gas (e.g., in a metal), the Fermi energy corresponds to the highest occupied energy state at absolute zero temperature ($T = 0$ K). As the temperature increases, the available states above $E_F$ remain largely unoccupied, and electrons added to the system occupy energy levels just above $E_F$. This makes the energy required to add an electron approximately equal to $E_F$ even at $T > 0$ K.

Since adding a few electrons to a system with a large number of particles does not significantly change its total energy, the **Fermi level** remains roughly constant. However, in quantum systems or devices with a small number of electrons, this approximation breaks down. In such cases, the statistical description of electrons as a gas no longer applies, and while the **Fermi energy** may not remain a fundamental parameter, the concept of **chemical potential** still holds and plays an important role.

### Non-Degenerate Semiconductors

In **non-degenerate semiconductors**, where the number of electrons in the conduction band is much smaller than the available states, the **Fermi-Dirac distribution** simplifies to the **Boltzmann distribution**. Here, the Fermi energy does not correspond to any occupied state, yet it still represents the electrochemical potential.

Electron and hole concentrations in semiconductors depend on the difference between the **Fermi energy** and the **conduction band energy** $E_C$. For instance:

$$
n = n_i \exp\left(\frac{E_F - E_C}{k_B T}\right)
$$

This difference $E_F - E_C$ plays a crucial role in determining the number of occupied states in the conduction band and the electron population.

### Electrochemical and Internal Chemical Potentials

While the total electrochemical potential is related to the total free energy of the system and remains constant at equilibrium, the **internal chemical potential** refers to the energy difference within the system and is linked to the **internal distribution** of electrons. The internal chemical potential can vary spatially.

The derivative of the internal chemical potential $E_F - E_C$ with respect to position leads to a **diffusion current**:

$$
\frac{\partial (E_F - E_C)}{\partial x} \neq 0 \quad \text{(diffusion current)}
$$

When the gradient of $E_C$ is not zero, we have a **drift current** due to the electric field $E$:

$$
-q \nabla \varphi = q \mathbf{E} \neq 0 \quad \text{(drift current)}
$$

At equilibrium, the total current is the sum of drift and diffusion components, and these currents cancel each other out, resulting in zero net current:

$$
\frac{\partial E_F}{\partial x} = 0
$$

### Example: Semiconductor at Equilibrium

In the example of a non-homogeneous semiconductor at equilibrium (as depicted in Fig. 3.7), the Fermi energy $E_F$ remains constant, but both $E_F - E_C$ and $E_C$ vary with position. This variation ensures the system maintains thermodynamic equilibrium through a balance of drift and diffusion currents. In this case, the electron concentration is non-uniform, with more electrons present in regions where the distance between $E_F$ and $E_C$ is larger.

By adjusting the position of $E_C$ via an applied electrostatic potential, the electron carrier concentration can be manipulated in an electronic device. This principle is central to the operation of devices like **Field Effect Transistors (FETs)** and, specifically, **MOSFETs**.
