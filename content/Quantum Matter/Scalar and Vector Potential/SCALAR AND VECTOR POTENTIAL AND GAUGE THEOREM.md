For this note you may want to reference this other notes: [[NABLA OPERATOR AND IT'S OPERATIONS|nabla]] and [[ELECTROMAGNETIC FIELDS|Maxwell equations]].
In this lecture we provided a detailed exploration of scalar and vector potentials in electromagnetism, emphasizing their role in both classical and quantum systems. The core objective of the lecture is to demonstrate that while electric and magnetic fields ($\mathbf{E}$ and $\mathbf{B}$) are the measurable physical quantities, the **scalar potential** ($\phi$) and **vector potential** ($\mathbf{A}$) from which they derive are more fundamental, flexible, and reveal deeper symmetries in physics—particularly through the concept of **gauge invariance**.

## 1. Electric Field and Scalar Potential

The lecture begins by discussing the electric field $\mathbf{E}$, traditionally described through **Gauss's law** for electricity:

$$
\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}
$$

where $\rho$ is the charge density, and $\varepsilon_0$ is the permittivity of free space. In electrostatics (where $\mathbf{B}$ is absent or constant), **Faraday’s law** tells us:

$$
\nabla \times \mathbf{E} = 0
$$

This implies that $\mathbf{E}$ is a **conservative field**, meaning the line integral of $\mathbf{E}$ around any closed path is zero, leading to the important result:

$$
\mathbf{E} = -\nabla \phi
$$

Here, $\phi$ is the **scalar potential** of the electric field, and the minus sign ensures that the electric field points in the direction of decreasing potential. Physically, the scalar potential $\phi$ represents the **energy per unit charge** at a point in space, or the work needed to move a unit charge from infinity to that point against the electric field.

This formulation is essential for solving problems in electrostatics, where determining $\phi$ via integration greatly simplifies the task of finding $\mathbf{E}$. Importantly, $\phi$ is defined only up to a constant—this reflects the fact that the absolute potential is irrelevant; only potential differences have physical meaning.

## 2. Magnetic Field and Vector Potential

The lecture then turns to the magnetic field $\mathbf{B}$, which, unlike $\mathbf{E}$, is **non-conservative**. According to **Ampere’s law** (in the absence of displacement current):

$$
\nabla \times \mathbf{B} = \mu_0 \mathbf{J}
$$

where $\mathbf{J}$ is the current density. Since the magnetic field is not irrotational, we cannot express $\mathbf{B}$ as the gradient of a scalar function. Instead, it is defined in terms of the **vector potential** $\mathbf{A}$, via the following relation:

$$
\mathbf{B} = \nabla \times \mathbf{A}
$$

This means that the magnetic field is the curl of a vector field, and the vector potential $\mathbf{A}$ is analogous to the scalar potential $\phi$, but for the magnetic field. The introduction of $\mathbf{A}$ provides a more versatile framework for analyzing electromagnetic systems, particularly in cases involving time-varying fields.

Just as the scalar potential $\phi$ is defined up to a constant, the vector potential $\mathbf{A}$ is defined up to the gradient of an arbitrary scalar function $\chi$. This gives rise to the concept of **gauge invariance**, which will be discussed shortly.

## 3. Time-Varying Fields: The General Case

The lecture then moves on to time-varying fields, where the interaction between the electric and magnetic fields becomes more complex. **Faraday’s law of induction** describes how a time-varying magnetic field generates an electric field:

$$
\nabla \times \mathbf{E} = -\frac{\partial \mathbf{B}}{\partial t}
$$

By substituting the expression $\mathbf{B} = \nabla \times \mathbf{A}$ into Faraday’s law, we get:

$$
\nabla \times \mathbf{E} = -\nabla \times \frac{\partial \mathbf{A}}{\partial t}
$$

This implies that the electric field is no longer simply the negative gradient of $\phi$, but must also account for the time derivative of the vector potential:

$$
\mathbf{E} = -\nabla \phi - \frac{\partial \mathbf{A}}{\partial t}
$$

This equation is crucial because it shows that the electric field is influenced by both the scalar potential $\phi$ and the time rate of change of the vector potential $\mathbf{A}$. In other words, in the presence of a time-varying magnetic field, the electric field becomes **non-conservative**, and we must account for both potentials to describe it fully.

## 4. Gauge Invariance and Freedom

The concept of **gauge invariance** is one of the central themes of the lecture. It arises because the potentials $\phi$ and $\mathbf{A}$ are not uniquely determined by the fields $\mathbf{E}$ and $\mathbf{B}$. Specifically, we can perform a **gauge transformation**:

$$
\mathbf{A}' = \mathbf{A} + \nabla \chi
$$

$$
\phi' = \phi - \frac{\partial \chi}{\partial t}
$$

where $\chi$ is any arbitrary scalar function. These transformations leave the electric and magnetic fields unchanged:

$$
\mathbf{E}' = -\nabla \phi' - \frac{\partial \mathbf{A}'}{\partial t} = \mathbf{E}
$$

$$
\mathbf{B}' = \nabla \times \mathbf{A}' = \mathbf{B}
$$

Thus, the physical fields $\mathbf{E}$ and $\mathbf{B}$ remain the same, even though the potentials may be transformed. This **gauge freedom** provides great flexibility in choosing the form of $\mathbf{A}$ and $\phi$ to simplify calculations, a technique commonly used in both classical electromagnetism and quantum mechanics.

For instance, one common gauge choice is the **Coulomb gauge**, where $\nabla \cdot \mathbf{A} = 0$. This choice simplifies the vector potential in certain scenarios, particularly in the analysis of radiation fields.

## 5. Physical Meaning of the Potentials

Initially, the potentials were introduced as convenient mathematical tools for solving Maxwell’s equations. However, the lecture emphasizes that these potentials—particularly the **vector potential** $\mathbf{A}$—have real **physical meaning**. One example of this is the relationship between the vector potential and the **momentum** of charged particles. The canonical momentum $\mathbf{p}_{\text{canonical}}$ is related to the mechanical momentum $m\mathbf{v}$ and the vector potential $\mathbf{A}$ by the following equation:

$$
\mathbf{p}_{\text{canonical}} = m\mathbf{v} + q\mathbf{A}
$$

This equation demonstrates that the vector potential directly influences the momentum of a charged particle, thereby affecting its motion in a magnetic field.

In quantum mechanics, the vector potential plays an even more significant role. The wave function $\psi$ of a particle is affected by the presence of $\mathbf{A}$ through **gauge transformations**, which introduce a phase shift:

$$
\psi' = \psi e^{iq\chi/\hbar}
$$

This phase shift has observable consequences, as seen in the **Aharonov-Bohm effect**, where charged particles are influenced by a magnetic vector potential even in regions where the magnetic field $\mathbf{B} = 0$. This effect shows that $\mathbf{A}$ is not merely a mathematical convenience but has profound physical implications, particularly in quantum systems.

## 6. The Schrödinger Equation and Potentials

The Schrödinger equation for a particle in the presence of electromagnetic fields includes the potentials $\phi$ and $\mathbf{A}$. Expanding the Schrödinger equation in the presence of a magnetic field, we obtain:

$$
\left\{ \frac{1}{2m} \left( \hat{p} - q\mathbf{A} \right)^2 + q\phi \right\} \psi = -i\hbar \frac{\partial \psi}{\partial t}
$$

### Kinetic Energy Term: $\frac{1}{2m} \left( \hat{p} - q\mathbf{A} \right)^2$

This term represents the **kinetic energy** of the particle in the presence of a magnetic field, but it is modified compared to the kinetic energy of a free particle.

- **$\hat{p}$** is the **canonical momentum operator**: $\hat{p} = -i\hbar \nabla$. It describes the momentum of a particle in free space. However, in an electromagnetic field, the particle’s momentum is modified by the vector potential $q\mathbf{A}$, representing the interaction between the charge $q$ and the magnetic field.
  
- The term $\left( \hat{p} - q\mathbf{A} \right)$ represents the **mechanical momentum** of the particle in the field, demonstrating how the magnetic field alters the particle’s motion, as discussed earlier in relation to $\mathbf{p}_{\text{canonical}} = m\mathbf{v} + q\mathbf{A}$.

Squaring this expression gives the kinetic energy in the field, representing both the particle's own motion and the interaction with the magnetic field.

### Electric Potential Energy Term: $q\phi$

This term represents the **potential energy** due to the **electric field**. The scalar potential $ \phi $ is related to the electric field by $\mathbf{E} = -\nabla \phi - \frac{\partial \mathbf{A}}{\partial t}$. This term expresses the **electrostatic energy** of the particle, directly linking to earlier discussions on how $\phi$ represents the energy per unit charge or the work needed to move a charge in the electric field.

### Hamiltonian Form: $\hat{H}\psi = -i\hbar \frac{\partial \psi}{\partial t}$

The entire left-hand side of the equation is the **Hamiltonian** $\hat{H}$, describing the system's total energy (both kinetic and potential). The right-hand side describes the time evolution of the wave function $\psi$, showing how the particle’s quantum state evolves under the influence of the fields.

### Full Interpretation of the Schrödinger Equation

This equation describes the behavior of a quantum particle in the presence of electric and magnetic fields. The kinetic energy is influenced by the magnetic field through $\mathbf{A}$, while the electric potential energy is influenced by $\phi$. These potentials play a fundamental role in shaping both the energy and the momentum of the particle. Furthermore, the equation shows how the potentials govern the time evolution of the quantum state, linking back to the earlier discussions on the physical significance of $\mathbf{A}$ and $\phi$.


