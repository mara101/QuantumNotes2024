
The oxidation of silicon involves the reaction of silicon atoms on the wafer surface with oxygen or steam to form silicon dioxide (SiO₂). This process can be achieved through two primary methods: dry oxidation and wet oxidation.

- **Dry oxidation**: This method uses oxygen (O₂) as the oxidizing agent. It results in a high-quality oxide layer with excellent electrical properties. However, the growth rate of the oxide layer in dry oxidation is relatively slow. The chemical reaction involved is:
  
  $$ \text{Si} + O_2 \rightarrow \text{SiO}_2 $$

- **Wet oxidation**: In this method, water vapor (H₂O) is used as the oxidizing agent, resulting in a faster oxide growth compared to dry oxidation. The reaction here is:

  $$ \text{Si} + 2H_2O \rightarrow \text{SiO}_2 + 2H_2 $$

Wet oxidation is typically used when a thicker oxide layer is required because it allows for faster oxidation rates, although the quality of the oxide may not be as high as that produced by dry oxidation because of impurities that derive from the H atom in the water molecule.

## Application of Silicon Dioxide in Microelectronics

Silicon dioxide has several critical functions in microelectronics:
- **Insulation**: SiO₂ acts as an insulator between different conducting regions of an integrated circuit, preventing electrical shorts and improving device performance. Note that is the **primary reason** why historically has been chosen silicon over others semiconductors, because silicon is the less problematic to oxidase and transform it in an insulator. 
- **Passivation**: The oxide layer protects the underlying silicon from contamination and environmental factors. It helps prevent the diffusion of impurities into the silicon substrate, which could alter its electrical properties.

## Model for Thermal Oxidation of Si

The Deal-Grove model provides a mathematical description of silicon oxidation kinetics. The model assumes two main processes that drive oxide growth: **diffusion of oxidants** through the oxide layer and **reaction at the silicon-oxide interface**. That means that the oxidant must diffuse in the entire thickness of the SiO₂ layer, so the more thick the more time will be required to arrive at the Silicon surface.
This is because the Silicon oxidation is a **diffusion process and not a deposition**.
![[Screenshot_20241014_113928.png|300x300]]
(Only b is correct)

The aim of the model presented is to predict two key variables: 
1. **The oxidation rate**, which is described by the time derivative of the oxide thickness $\frac{\partial x_{\text{ox}}(t)}{\partial t}$, and 
2. **The oxide thickness at any given time** $x_{\text{ox}}(t)$, which is the total amount of SiO₂ formed on the silicon surface after a given time.
![[Screenshot_20241016_134037.png|400x400]]
### Diffusion-Limited Process

The model operates under the assumption that silicon oxidation is primarily a **diffusion-limited process**. This means that the rate at which the oxide layer grows is limited not by the chemical reaction of oxygen or water with silicon, but by the rate at which the oxidant (either oxygen or water vapor) can diffuse through the already-grown oxide layer.

In this process, there are three critical fluxes:
1. **F1** – The flux of oxidant molecules in the gas phase (either oxygen or water vapor), which diffuse to the surface of the growing oxide film.
2. **F2** – The flux through the oxide, where the oxidant molecules diffuse through the already-formed SiO₂ layer to reach the interface between the oxide and the silicon.
3. **F3** – The reaction flux at the silicon interface, where the oxidant molecules finally react with silicon to form additional SiO₂.

At **steady state**, these fluxes must be equal, meaning $F1 = F2 = F3$. In other words, the amount of oxidant arriving at the surface must be equal to the amount diffusing through the oxide and also equal to the amount reacting with silicon at the interface. This balance ensures that the oxidation process proceeds consistently over time, but as the oxide layer thickens, the diffusion of oxidants through the layer becomes slower, which ultimately slows down the growth of the oxide.
### Fick’s First Law of Diffusion

The model for the thermal oxidation of silicon uses **Fick's first law of diffusion** to describe the diffusion of oxidant molecules through the growing oxide layer. According to Fick’s law, the flux of oxidant molecules through the oxide is given by:

$$ J = F_2 = -D \cdot \frac{dN}{dx} = D \cdot \left( \frac{N_0 - N_i}{x_0} \right) $$

Where:
- $J$ (or $F_2$) is the flux of oxidant molecules, measured in $\frac{\text{number of particles}}{\text{cm}^2 \cdot \text{sec}}$,
- $D$ is the **diffusivity** of the oxidant molecules in the silicon dioxide layer, measured in $\frac{\text{cm}^2}{\text{sec}}$,
- $N_0$ and $N_i$ are the concentrations of oxidant molecules at the outer surface and the silicon interface, respectively, measured in $\frac{\text{molecules}}{\text{cm}^3}$,
- $x_0$ is the thickness of the oxide layer, measured in $\text{cm}$.

### Oxidant Concentrations

- The oxidant concentration at the surface, $N_0$, depends on the type of oxidation (dry or wet) and the temperature:
  - For **dry oxidation** at 1000°C and 1 atm:  $N_0 = 5.2 \times 10^{16}$, $\frac{\text{molecules}}{\text{cm}^3}$,
  - For **wet oxidation** at 1000°C and 1 atm: $N_0 = 3 \times 10^{19} \, \frac{\text{molecules}}{\text{cm}^3}$.

### Reaction at the Silicon Interface

At the silicon interface, the reaction flux $F_3$ is proportional to the concentration of oxidant molecules at the interface, $N_i$. This can be expressed as:

$$ J = F_3 = k_s \cdot N_i $$

Where:
- $k_s$ is the **surface reaction rate constant**, representing the speed of the oxidation reaction at the silicon surface.

At steady state, the fluxes of the oxidant molecules must be equal:

$$ J = F_2 = F_3 $$
By combining Fick's law with the surface reaction rate equation and eliminating $N_i$, we can express the flux $J$ as:

$$ J = \frac{D \cdot N_0}{x_0 + \frac{D}{k_s}} $$

This equation describes the diffusion-limited flux of oxidant molecules through the growing oxide layer, incorporating both the diffusivity of the oxidant in the oxide and the reaction rate at the silicon interface.
### Derivation of the oxidation rate
Now we can define the oxidation rate as:
![[Screenshot_20241016_154431.png]]
So then we obtain the general relation for the silicon Oxidation:
![[Screenshot_20241016_155155.png|500]]
Where:
- $x_{\text{ox}}$ is the thickness of the oxide layer at time $t$,
- $B$ and $A$ are constants related to the physical parameters of the system (such as diffusivity and surface reaction rate),
- $\tau$ is a time shift introduced to account for the starting oxide thickness, $x_i$, from a previous oxidation step or an initial condition.

#### Key Parameters

1. **Starting Oxide Thickness**:
   - At time $t = 0$, the oxide thickness is $x_{\text{ox}}(t = 0) = x_i$, which represents the initial thickness of the oxide layer.

2. **Time Shift ($\tau$)**:
   - The time shift $\tau$ is calculated as:

   $$\tau = \frac{x_i^2}{B} + \frac{x_i}{\left( \frac{B}{A} \right)}$$

   This term accounts for the initial thickness $x_i$ and shifts the time axis accordingly.

3. **Constants $A$ and $B$**:
   - $A = \frac{2 \cdot D}{k_s}$, where:
     - $D$ is the diffusivity of the oxidant species in the oxide layer,
     - $k_s$ is the surface reaction rate.
   
   - $B = \frac{2 \cdot D \cdot N_0}{N_{\text{ox}}}$, where:
     - $N_0$ is the concentration of oxidant at the oxide surface,
     - $N_{\text{ox}}$ is the concentration of oxidant in the oxide.

#### Solution to the Equation

The solution to the general equation that provides the oxide thickness as a function of time is:

$$x_{\text{ox}}(t) = \frac{1}{2} A \left[ \sqrt{1 + \frac{4 \cdot B}{A^2} (t + \tau)} - 1 \right]$$

This equation gives the thickness of the oxide layer $x_{\text{ox}}$ at any given time $t$, taking into account both the diffusion of oxidant molecules through the oxide and the reaction rate at the silicon interface. The equation shows how the oxide growth slows down over time as the layer thickens, following a non-linear behavior due to the increasing resistance to oxidant diffusion.


## Growth Rate Regimes for Silicon Oxidation

The growth of the silicon dioxide layer follows different regimes depending on the time and how it relates to the physical constants of the system. These regimes are derived from the general solution for the oxide thickness over time.

### Short Time Regime

At **short times**, when $(t + \tau) \ll \frac{A^2}{4 \cdot B}$, the solution can be simplified using a **Taylor series expansion**. In this case, the equation reduces to:

$$x_{\text{ox}}(t) = \left( \frac{B}{A} \right) \cdot (t + \tau)$$
- The growth rate is **linear** in this regime.
- The growth is **limited by the rate of the chemical reaction** between the oxidant molecules and silicon at the interface.
- The growth rate parameter is **B/A**, which represents the linear growth rate.
- The oxide thickness increases proportionally with time.

### Long Time Regime

At **long times**, when $(t + \tau) \gg \frac{A^2}{4 \cdot B}$, the equation simplifies to:

$$x_{\text{ox}}(t) = \sqrt{B \cdot (t + \tau)}$$
- The growth rate follows a **parabolic behavior** in this regime.
- The growth is **limited by the diffusion** of oxidant molecules through the growing oxide layer.
- The parameter $B$ represents the parabolic growth rate.
- The oxide thickness grows more slowly as time progresses due to the increasing difficulty for oxidants to diffuse through the thicker oxide layer.
![[Screenshot_20241016_161412.png]]





