# Time Invariant Maxwell Equations
In the static case we consider the [[ELECTROMAGNETIC FIELDS|Maxwell equations]] but simplified due to the fact that in the static case no time variance is allowed. In that case the Maxwell equations becomes:
$$\nabla \times \mathbf{H}(\mathbf{r}) = \mathbf{J}(\mathbf{r})$$
$$\nabla \times \mathbf{E}(\mathbf{r}) = 0$$
$$\nabla \cdot \mathbf{B}(\mathbf{r}) = 0$$
$$\nabla \cdot \mathbf{D}(\mathbf{r}) = \rho(\mathbf{r})$$


# Charge, Force, Potential Energy, and Electrostatic Potential

The concept of charge, force, potential energy, and electrostatic potential is foundational in electrostatics, describing the behavior of charges under the influence of electric fields.

When a charge $Q$ moves with velocity $\mathbf{v}$ in a region characterized by an electric field $\mathbf{E}$ and a magnetic field $\mathbf{H}$, it experiences a force $\mathbf{F}$. The total force on the charge is the superposition of two components: the **electric force** and the **Lorentz force**. Mathematically, this is expressed as:

$$
\mathbf{F} = Q \mathbf{E} + Q \mathbf{v} \times \mathbf{B}
$$

The term $Q \mathbf{E}$ represents the force exerted by the electric field, while $Q \mathbf{v} \times \mathbf{B}$ represents the Lorentz force caused by the interaction between the moving charge and the magnetic field. In many cases, particularly in semiconductor devices where magnetic effects are minimal, the Lorentz force is negligible. Hence, the focus often remains on the electric force, which is conservative.

For a conservative electric field (i.e., in electrostatic conditions), the electric force can be derived from the **electrostatic potential** $\phi(\mathbf{r})$. The relationship is given by:

$$
\mathbf{E} = -\nabla \phi(\mathbf{r})
$$

This indicates that the electric field is the negative gradient of the electrostatic potential, which implies that the field is irrotational (no circulation). The force on the charge due to the electric field becomes:

$$
\mathbf{F} = -Q \nabla \phi
$$

The **potential energy** associated with a charge $Q$ in an electrostatic potential $\phi$ is expressed as:

$$
U = Q \phi
$$

This relationship shows that the potential energy $U$ is directly proportional to both the charge $Q$ and the electrostatic potential $\phi$. For positive charges, the potential energy has the same sign as the electrostatic potential, while for negative charges (like electrons), the potential energy is of opposite sign.

Additionally, the total energy of a particle with mass $m$, charge $Q$, and velocity $\mathbf{v}$ consists of its **kinetic energy** and **potential energy**. The total energy is given by:

$$
E_{\text{tot}} = \frac{1}{2} m \mathbf{v}^2 + Q \phi
$$

In the case of electrons, which have a rest mass of $m_e = 9.1 \times 10^{-31} \, \text{kg}$ and an elementary charge $Q = -q$, where $q = 1.6 \times 10^{-19} \, \text{C}$, the energy gained by an electron when subjected to a voltage difference $\Delta \phi = 1 \, \text{V}$ is called an **electron volt (eV)**. One electron volt corresponds to the energy:

$$
1 \, \text{eV} = 1.6 \times 10^{-19} \, \text{J}
$$

This unit of energy is particularly convenient in solid-state physics and is commonly used when dealing with energies of charged particles in electric fields.


#### Flashcards 
Give the Maxwell Equations for the static case::[[ELECTROSTATIC, CHARGE,POTENTIAL ENERGY AND ELECTROSTATIC POTENTIAL]]
Give the complete Lorentz Force formula::[[ELECTROSTATIC, CHARGE,POTENTIAL ENERGY AND ELECTROSTATIC POTENTIAL]]
Express the Electric field in function of the electrostatic potential $\phi(x)$ and then express the force on a charge Q based on that knowledge::[[ELECTROSTATIC, CHARGE,POTENTIAL ENERGY AND ELECTROSTATIC POTENTIAL]]
Express the total energy of the particle in electromagnetism::[[ELECTROSTATIC, CHARGE,POTENTIAL ENERGY AND ELECTROSTATIC POTENTIAL]]


