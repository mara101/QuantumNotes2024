## Displacement Current in Semiconductors

Before discussing non-equilibrium phenomena in semiconductors, it's essential to complete our understanding of the current components by addressing **displacement current**. This type of current arises due to a time-varying electric field, rather than the movement of free charge carriers. The displacement current is expressed as:

$$
\mathbf{J}_{\text{disp}} = \frac{\partial \mathbf{D}}{\partial t}
$$

Here, $\mathbf{D}$ refers to the **dielectric displacement vector**, which relates to the electric field as $\mathbf{D} = \epsilon \mathbf{E}$. In this relationship, $\epsilon$ represents the dielectric permittivity of the material, and $\mathbf{E}$ is the electric field. Therefore, any change in the electric field over time produces a displacement current.

In general, **displacement current** is typically negligible in semiconductors because it does not involve the direct flow of electrons or holes. However, there are a few scenarios where this current becomes significant:

- **High-frequency operation**: Displacement current becomes relevant when a device operates at very high frequencies, or when it is exposed to fast-varying signals. At these high frequencies, the rapid oscillation of the electric field produces a notable displacement current.
  
- **Insulating materials**: In insulating materials, such as those found in capacitors, where there are no free carriers, **conduction current is nearly zero**. In these cases, displacement current can be the **primary current component**, as seen in the dielectric region of capacitors.

In cases where the electric field varies sinusoidally, for instance under **harmonic excitation**, the displacement current is given by:

$$
\mathbf{D} = \mathbf{D}_0 \sin(\omega t)
$$

Where:
- $\mathbf{D}_0$ is the amplitude of the dielectric displacement,
- $\omega = 2\pi f$ is the angular frequency, with $f$ representing the operating frequency.

The corresponding displacement current then becomes:

$$
\mathbf{J}_{\text{disp}} = \omega \mathbf{D}_0 \cos(\omega t)
$$

This equation shows that the displacement current is directly proportional to the operating frequency ($\omega$), meaning that at higher frequencies, the displacement current increases. 

In devices like **capacitors**, where the dielectric material separates the conductive plates, the displacement current plays a crucial role because the **conduction current is negligible** due to the absence of free carriers. The oscillating electric field between the capacitor plates generates a displacement current, which sustains the electric circuit even though no charge physically moves through the dielectric.

## Thermal Equilibrium and Non-Equilibrium Conditions in Semiconductors

In semiconductor devices, **thermal equilibrium** is defined as the state where there is no exchange of energy between the system and its environment. In this state, the carrier concentrations (electrons and holes) remain constant over time, and no current flows through the material. However, **thermal equilibrium** is not the typical operating condition for semiconductor devices. Most electronic devices, whether digital or analog, operate out of equilibrium to perform functions such as signal amplification, logic state switching, or other transformations of electrical signals.

### Non-Equilibrium and Free Carrier Variations

When a semiconductor operates out of equilibrium, the **free carrier concentrations**—that is, the densities of electrons ($n$) and holes ($p$)—deviate from their equilibrium values. These variations can occur both in **space** and **time**, meaning that electron and hole densities may become functions of position $x$ and time $t$:

$$
n = n(x,t), \quad p = p(x,t)
$$

For simplicity, these spatial variations are typically considered along one dimension, usually denoted as the $x$-axis.

### Causes of Non-Equilibrium Carrier Concentrations

The deviations in carrier concentrations away from equilibrium are caused by several factors:

- **Diffusion**: Free carriers move from regions of high concentration to regions of lower concentration, generating a **diffusion current**.
- **Drift**: Carriers move under the influence of an electric field, resulting in a **drift current**.
- **Displacement Current**: As discussed previously, a **displacement current** can arise due to a time-varying electric field. This current is usually negligible compared to drift and diffusion currents, except at very high frequencies (e.g., above 100 GHz) or in insulating materials where there are no free carriers.
- **Generation and Recombination (GR)**: Free carrier concentrations are also influenced by the processes of **generation** (creation of electron-hole pairs) and **recombination** (destruction of electron-hole pairs).

### Excess Carrier Concentrations and Low Injection Levels

When the system moves out of equilibrium, the **excess carrier concentrations** are defined as the difference between the carrier concentrations at any given time and their equilibrium values:

$$
n'(x, t) = n(x, t) - n_0(x), \quad p'(x, t) = p(x, t) - p_0(x)
$$

Here, $n_0(x)$ and $p_0(x)$ represent the electron and hole concentrations under thermal equilibrium, and $n'(x, t)$ and $p'(x, t)$ denote the **excess** carrier concentrations. These excess concentrations can be positive (indicating **injection** of charge carriers) or negative (indicating **depletion**).

In certain cases, especially in bipolar devices, the doping type of the region is denoted explicitly. For example:
- $n_p(x, t)$, $p_p(x, t)$ in a **p-type region**
- $n_n(x, t)$, $p_n(x, t)$ in an **n-type region**

In these cases, the corresponding excess densities are:

$$
n_p'(x, t) = n_p(x, t) - n_{p0}, \quad p_p'(x, t) = p_p(x, t) - p_{p0}
$$

in a p-type region, and similarly:

$$
n_n'(x, t) = n_n(x, t) - n_{n0}, \quad p_n'(x, t) = p_n(x, t) - p_{n0}
$$

in an n-type region.

### Low Injection Approximation

In a uniformly doped semiconductor, **local charge neutrality** means that the positive and negative charges within the material balance out. This is expressed by:

$$
\rho_0 = q(p_0 - n_0 + N_D - N_A) = 0
$$

where:
- $p_0$ and $n_0$ are the equilibrium concentrations of holes and electrons,
- $N_D$ is the donor concentration (positive fixed charge from donors),
- $N_A$ is the acceptor concentration (negative fixed charge from acceptors),
- $\rho_0$ is the net charge density at equilibrium,
- $q$ is the elementary charge.

This equation indicates that, at thermal equilibrium, the net charge density $\rho_0$ is zero, meaning that the material is electrically neutral.

Even when the system is out of equilibrium (for example, when excess carriers are injected), the **quasi-neutrality condition** often still holds. This means that the net charge density remains close to zero:

$$
\rho = q(p - n + N_D - N_A) \approx 0
$$

Here, $p$ and $n$ are the nonequilibrium concentrations of holes and electrons, respectively. Under this condition, the excess carrier densities for electrons and holes (the additional carriers injected into the system) tend to be similar:

$$
p' \approx n'
$$

Now, consider an **n-type semiconductor** doped with donor atoms at a concentration $N_D$. At **thermal equilibrium**, the majority carrier concentration (electrons) is approximately equal to the donor concentration:

$$
n_{n0} \approx N_D, \quad p_{n0} \approx \frac{n_i^2}{N_D}
$$

where $n_i$ is the intrinsic carrier concentration. The majority carriers in this n-type material are electrons, and the minority carriers are holes.

When the sample is taken **out of equilibrium** by introducing excess carriers (due to injection, optical excitation, or another mechanism), we refer to the situation as **low injection** if the excess carrier concentrations are **much smaller** than the equilibrium concentration of the majority carriers:

$$
n_n', p_n' \ll n_{n0} = N_D
$$

In this regime, the excess minority carriers (holes in an n-type material) are significantly perturbed, while the majority carrier concentration (electrons) remains almost unchanged. This condition simplifies the analysis because:

- The minority carrier concentration changes considerably from its equilibrium value, becoming much larger than its equilibrium level.
- The majority carrier concentration stays close to its equilibrium value.

Thus, in **low injection**, the **minority carriers** (holes in an n-type material or electrons in a p-type material) are affected much more significantly than the **majority carriers**, which remain relatively stable:

$$
p_p \approx p_{p0}, \quad n_n \approx n_{n0}
$$

This approximation allows us to focus primarily on the behavior of the minority carriers, making the mathematical treatment of the system simpler. It is often used in semiconductor device modeling, especially in cases where the excess carrier concentrations are small.
![[Screenshot_20241020_125128.png]]
The image provides a visual representation of how carrier concentrations change in an n-type semiconductor under low and high injection conditions. In **low injection**, only the minority carrier concentration increases significantly, while in **high injection**, both carrier types (electrons and holes) are affected, and their concentrations become comparable.
### High Injection Level

In contrast, **high injection** occurs when the excess carrier concentrations ($n'$ and $p'$) become comparable to the equilibrium **majority carrier** concentration. In this case, both the majority and minority carrier populations are significantly perturbed. This leads to more complex behaviors, as both carrier types must be taken into account when analyzing the system's electrical properties.

## Generation and Recombination (GR) Phenomena in Semiconductors

In semiconductors, **generation** and **recombination** (GR) refer to the processes by which free carriers, specifically **electrons** and **holes**, are created and destroyed. These processes are fundamental to the operation of semiconductor devices, as they directly impact the availability of charge carriers that are essential for conducting electric current. 

- **Generation** occurs when electrons gain enough energy to jump from the **valence band** to the **conduction band**, creating an electron-hole pair. The electron, now in the conduction band, is free to move, while the hole left behind in the valence band acts as a positive charge carrier.
- **Recombination** is the reverse process: an electron in the conduction band loses energy and falls back into a hole in the valence band, eliminating both the electron and the hole. This process restores the system to a lower energy state.

### Mechanisms of Generation and Recombination
![[Screenshot_20241020_151235.png]]
There are several mechanisms by which generation and recombination occur, and these can be broadly classified based on the nature of the energy transitions involved.

1. **Direct (Band-to-Band) Transitions**:
   - In **direct transitions**, electrons move directly between the conduction band and the valence band without passing through intermediate energy states. These transitions involve a direct exchange of energy between the electron and the lattice or external factors like photons.
   - Examples of direct transitions include:
     - **Thermal generation and recombination**, which occur naturally at any temperature above absolute zero due to the thermal agitation of the semiconductor lattice.
     - **Auger recombination**, where an electron-hole pair recombines, and the excess energy is transferred to a third carrier (another electron or hole) instead of being released as a photon.
     - **Impact ionization**, where a high-energy carrier collides with an atom and creates additional electron-hole pairs.
     - **Radiative recombination**, where an electron falls from the conduction band to the valence band, emitting a photon. This process is the basis for the operation of **light-emitting devices** such as LEDs and lasers.
   
   In direct transitions, energy is directly exchanged between the bands, and no intermediate steps are involved (as illustrated on the left side of Figure 3.10).

2. **Indirect (Trap-Assisted) Transitions**:
   - **Indirect transitions** occur when an electron moves between the conduction and valence bands, but the transition involves one or more intermediate energy states within the bandgap. These energy states, known as **trap levels**, are typically introduced by impurities or defects in the semiconductor lattice.
   - The most common form of indirect recombination is **Shockley-Read-Hall (SRH) recombination**, named after the physicists who developed a widely used model to describe this process. In SRH recombination, an electron from the conduction band is first captured by a trap state, and then recombines with a hole in the valence band (or vice versa).
   - This type of recombination is especially important in **indirect bandgap semiconductors** like **silicon**, where direct band-to-band transitions are less likely to occur. In such materials, trap-assisted recombination is often the dominant mechanism.
### Quantifying Generation and Recombination

To describe generation and recombination quantitatively, two key rates are used:
- **Generation rate** ($G_n$ for electrons and $G_p$ for holes): This represents the number of electrons or holes generated per unit volume per unit time.
- **Recombination rate** ($R_n$ for electrons and $R_p$ for holes): This is the number of electrons or holes that recombine per unit volume per unit time.

The **net recombination rate** is the difference between the recombination rate and the generation rate for each type of carrier:

$$
U_n = R_n - G_n
$$

$$
U_p = R_p - G_p
$$

At **thermal equilibrium**, the system is stable, and there is no net change in the carrier populations. This means that the generation and recombination rates are balanced, so the net recombination rate is zero:

$$
U_{n0} = 0, \quad U_{p0} = 0
$$

### Lifetime Approximation

To simplify the analysis of GR phenomena, particularly in cases where an **analytical approach** is preferred, the **lifetime approximation** is commonly used. This model relates the excess carrier concentrations to the **carrier lifetime**, which is the average time a free carrier exists before recombining.

In this approximation, the **net recombination rate** can be expressed as:

$$
U_n \approx \frac{n' - n_0}{\tau_n}
$$

$$
U_p \approx \frac{p' - p_0}{\tau_p}
$$

Where:
- $n'$ and $p'$ are the non equilibrium concentrations of electrons and holes.
- $n_0$ and $p_0$ are the equilibrium concentrations.
- $\tau_n$ and $\tau_p$ are the **electron** and **hole lifetimes**, respectively, representing the average time before recombination occurs.

This approximation simplifies the complex mathematical treatment of GR phenomena by focusing on the relationship between excess carriers and their average lifetimes.

