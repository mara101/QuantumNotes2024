## Continuity Equations

The **continuity equations** describe the dynamics of **free carriers** (electrons and holes) in a semiconductor. These equations are derived from the principle of **particle conservation**, which states that the total number of electrons and holes within a given volume must account for particles entering, exiting, being generated, or recombining within that volume.

To derive the continuity equations, consider a small elementary volume $dV = A \cdot dx$ of a semiconductor, where:
- $A$ is the cross-sectional area.
- $dx$ is the thickness along the $x$-axis, which is the direction of the carrier flow.

Within this volume, changes in carrier concentrations arise from four components:
1. **Particles entering** from one side of the volume at position $x$.
2. **Particles exiting** from the opposite side at position $x + dx$.
3. **Generation** of particles within the volume.
4. **Recombination** of particles within the volume.

#### Electron and Hole Continuity Equations
![[Screenshot_20241020_152901.png]]
For **electrons**, the continuity equation relates the change in electron concentration $n$ over time to the current density of electrons $J_n$, the [[DISPLACEMENT CURRENT AND OFF-EQUILIBRIUM SEMICONDUCTOR BEHAVIORS|generation]] rate $G_n$, and the recombination rate $R_n$. Similarly, the equation for **holes** is defined using the hole concentration $p$, current density $J_p$, generation rate $G_p$, and recombination rate $R_p$.

The algebraic combination of all components gives:

$$
A \cdot dx \cdot \frac{\partial n}{\partial t} = - \frac{A}{q} \left( J_n(x + dx) - J_n(x) \right) + A \cdot dx \cdot (G_n - R_n)
$$

Similarly, for holes:

$$
A \cdot dx \cdot \frac{\partial p}{\partial t} = \frac{A}{q} \left( J_p(x + dx) - J_p(x) \right) + A \cdot dx \cdot (G_p - R_p)
$$

By taking the limit as $dx \to 0$, we get the **one-dimensional continuity equations** for electrons and holes:

$$
\frac{\partial n}{\partial t} = \frac{1}{q} \frac{\partial J_n}{\partial x} - U_n
$$

$$
\frac{\partial p}{\partial t} = - \frac{1}{q} \frac{\partial J_p}{\partial x} - U_p
$$

where $U_n = R_n - G_n$ and $U_p = R_p - G_p$ are the **net recombination rates** for electrons and holes, respectively.

#### Gauss’s Law and Charge Density

To fully describe the behavior of the system, the continuity equations must be coupled with an equation for the electric field. This is done through **Gauss’s law**, which relates the electric field $E$ to the total charge density $\rho$:

$$
\frac{\partial E}{\partial x} = \frac{\rho}{\epsilon}
$$

where $\rho = q(p - n + N_D - N_A)$ (watch [[DISPLACEMENT CURRENT AND OFF-EQUILIBRIUM SEMICONDUCTOR BEHAVIORS|here]] to see where the formula comes from), and $N_D$ and $N_A$ represent the concentrations of donor and acceptor impurities, respectively. This equation can be rewritten in terms of the **electrostatic potential** $\varphi$, which is related to the electric field by:

$$
E = - \frac{\partial \varphi}{\partial x}
$$

#### Complete Semiconductor Model

The **semiconductor mathematical model** in one dimension consists of three key **partial differential equations** that describe the behavior of the system:
1. The **electron continuity equation**:
   $$
   \frac{\partial n}{\partial t} = \frac{1}{q} \frac{\partial J_n}{\partial x} - U_n
   $$
   
2. The **hole continuity equation**:
   $$
   \frac{\partial p}{\partial t} = - \frac{1}{q} \frac{\partial J_p}{\partial x} - U_p
   $$
   
3. **Gauss's law** (expressed using the electrostatic potential):
   $$
   \frac{\partial^2 \varphi}{\partial x^2} = -\frac{\rho}{\epsilon}
   $$

These equations are completed by **constitutive relations** that describe how the current densities depend on carrier concentrations, electric fields, and the gradients of the carrier concentrations. These relations are:

- For electrons:
  $$
  J_n = q n \mu_n E + q D_n \frac{\partial n}{\partial x}
  $$
  
- For holes:
  $$
  J_p = q p \mu_p E - q D_p \frac{\partial p}{\partial x}
  $$

Here, $\mu_n$ and $\mu_p$ are the mobilities of electrons and holes, and $D_n$ and $D_p$ are their diffusion coefficients.

The set of equations described is commonly referred to as the [[SEMICONDUCTOR FREE CARRIER MOTION|drift-diffusion model]], which is fundamental in semiconductor device modeling. 
## Mathematical Model Approximations in Semiconductors

In the general case, especially for **multi-dimensional** semiconductor problems, the mathematical model describing the behavior of charge carriers is highly complex. Such models typically require **numerical solutions**, often implemented using specialized **Technology CAD (TCAD)** tools, or **physical device simulators**. These tools solve the equations computationally, handling the detailed physics of semiconductor devices. However, to gain a more intuitive understanding of device behavior without requiring computational solutions, it is common to apply certain approximations to simplify the mathematical model, allowing for **analytical solutions**.

The key **approximations** made in simplified models include:

- **Constant electron and hole mobility**: The mobilities of electrons and holes are assumed to be constant, corresponding to their low-field values.
- **Carrier diffusivity**: The diffusivity of carriers is derived from the [[SEMICONDUCTOR FREE CARRIER MOTION|Einstein relation]]: 
  $$
  D = V_T \mu
  $$
  where $V_T$ is the **thermal voltage**, and $\mu$ is the carrier mobility.
- **Lifetime approximation for generation and recombination**: Carrier generation and recombination are described using the **lifetime approximation**, where the net recombination rates depend on the carrier concentrations and their respective lifetimes.
- **Complete ionization of dopants**: It is assumed that all dopant atoms are completely ionized, meaning that each donor atom contributes one electron and each acceptor atom contributes one hole.

With these approximations, the continuity equations for electrons and holes simplify to:

$$
\frac{\partial n}{\partial t} = \mu_n \frac{\partial (nE)}{\partial x} + D_n \frac{\partial^2 n}{\partial x^2} - \frac{n - n_0}{\tau_n}
$$

$$
\frac{\partial p}{\partial t} = -\mu_p \frac{\partial (pE)}{\partial x} + D_p \frac{\partial^2 p}{\partial x^2} - \frac{p - p_0}{\tau_p}
$$

And Gauss's law becomes:

$$
\frac{\partial^2 \varphi}{\partial x^2} = - \frac{q}{\epsilon} (p - n + N_D - N_A)
$$

These simplified equations provide a good balance between capturing the essential behavior of semiconductor devices while remaining analytically solvable.

#### Neutral Regions

A **neutral region** in a semiconductor is one where the **net charge density** is zero, meaning that the positive and negative charges balance out perfectly. Mathematically, this condition is expressed as:

$$
\rho = 0
$$

In a **one-dimensional model**, **Gauss’s law** tells us that in a neutral region, the **electric field** must be **constant**. This constant electric field is denoted as:

$$
E(x) = E_0
$$

Since the electric field is constant, the **electrostatic potential** becomes a **linear function** of position. This linear relationship between the electric field and potential is expressed as:

$$
\varphi(x) = -E_0 x + \varphi_0
$$

The **potential difference** between two points $x_1$ and $x_2 = x_1 + d$ in the neutral region can be calculated from this equation:

$$
\Delta \varphi = \varphi(x_2) - \varphi(x_1) = -E_0 d
$$

If the electric field within the neutral region is **zero** ($E_0 = 0$), it follows that the **potential difference** across the region is also zero. In this case, the **drift current** (the current due to the motion of carriers under the influence of the electric field) vanishes, as there is no electric field to drive it.

When the drift current is negligible, the **continuity equations** for electrons and holes are **decoupled**, simplifying the mathematical model to just:

$$
\frac{\partial n}{\partial t} = D_n \frac{\partial^2 n}{\partial x^2} - \frac{n - n_0}{\tau_n}
$$

$$
\frac{\partial p}{\partial t} = D_p \frac{\partial^2 p}{\partial x^2} - \frac{p - p_0}{\tau_p}
$$

These equations describe **diffusion currents** as the only mechanism of carrier movement, meaning that the carriers move due to concentration gradients rather than an electric field.

This scenario simplifies the analysis of semiconductor devices in regions where charge neutrality holds. In contrast, if the potential difference across the region is **non-zero** (i.e., an electric field is present), **drift currents** must be considered, as the carriers are influenced by both the electric field and diffusion processes. Therefore, the inclusion of the electric field complicates the analysis, as it requires solving the full drift-diffusion model.





