The **Free Electron Fermi Gas** model is a cornerstone in solid-state physics that helps to explain the behavior of conduction electrons in metals. This model assumes that conduction electrons in metals form a gas of non-interacting fermions that obeys Fermi-Dirac statistics. The model combines classical free electron theory with quantum mechanics and provides key insights into the distribution of electron energies and the structure of metals at absolute zero and finite temperatures.

## Initial Conditions 
This model begins with applying two important  conditions:
- The electrons are **Independent** from each others. That means that the Coulomb repulsion forces between electrons can be neglected.
- The electrons are **Free** and that means that we consider an electrostatic potential $V(x) = 0$ for every point.

Also we don't want to consider the possibility of getting out of the lattice of the solid, so we apply also the **periodic boundary condition** (PBC) or **Born Von Karman condition**. 
$$\Psi(x, y, z) = \Psi(x + L_x, y, z) = \Psi(x, y + L_y, z) = \Psi(x, y, z + L_z)
$$
![[Screenshot_20241013_153508.png]]
This condition ensures that the wavefunction $\Psi$ is periodic in all three spatial dimensions x, y, and z, with $L_x$​, $L_y$, and $L_z$​ being the macroscopic dimensions of the system in the respective directions. It implies that when an electron reaches one boundary of the system, it reappears at the opposite boundary, simulating an infinite crystal lattice.

## Consideration
Now if we consider the periodic boundaries condition above we observe that if the electron escapes the macroscopic volume, finds himself again in the same volume, giving the illusion of being confined in the same volume. So this type of example is similar to the [[THE INFINITE SQUARE WELL|infinite Square Well]]. 
In fact we can say that the [[SCHRODINGER EQUATION|Schrodinger Equation]] can be written in the form:

$$-\frac{\hbar}{2m} \nabla^{2} \Psi(\bar{r}) = E \Psi (\bar{r})$$
Because the Hamiltonian operator does not consider the Potential energy that we considered 0 previously for every point.
Then we can write the general solution as:
$$
\Psi(\bar{r}) = \frac{1}{\sqrt{ \mathbf{V} }} e^{ i \bar{k} \bar{r} } \quad (\mathbf{V} = L_{x} \cdot L_{y} \cdot L_{z}) \tag{1}
$$
with eigenvalues for the energy as:
$$
E = \frac{\hbar^{2} k^{2}}{2m}
$$
![[Screenshot_20241016_112645.png]]

Now ,as we said before, in this case we are considering a periodic boundary condition and we can equate the solution that we have just found as:
$$
\displaylines{
\frac{1}{\sqrt{ V}} e^{ i(k_{x} x + k_{y} y + k_{z} z) } = \underbrace{ \frac{1}{\sqrt{ V }} e^{ i(k_{x} x + k_{x} L_{x}+ k_{y} y + k_{z} z) } }_{ \Psi(x + L_{x}, y, z) } \\
\Downarrow \\
e^{ i k_{x} L_{x} } = 1 \\
\Downarrow \\
{\color{red} k_{x} L_{x} = 2 \pi n_{x}} 
}
$$
So we have just found that in order to maintain the boundaries conditions $k_xL_x = 2\pi n_x$ and so $k$ must be discrete and:
![[Screenshot_20241013_160218.png]]But the $L$ values are macroscopic values, but in compare $k$ is microscopic and can be considered as being continuous. 

## Objective
The objective of this model is to determine the quantities of charges in a crystal. This could be determinate with the following formula:

$$ 
n = \int D(E) f(E,T)\, dE 
$$
where:

- $n$ represents the total number of charge carriers in the crystal.
- $D(E)$ denotes the density of states.
- $f(E,T)$ corresponds to the Fermi-Dirac distribution for a given temperature $T$
![[Screenshot_20241013_180552.png]]

### Density of States Function
The **Density of States (DOS)** function, denoted as $D(E)$, describes how the number of available quantum states is distributed over a range of energy levels in a system. In the context of solid-state physics and free electron models, the DOS tells us how many electron states are available at each energy level in a material, particularly in metals, semiconductors, and insulators.
$$
D(E) = \frac{1}{V} \frac{dN(E)}{dE} \quad \left[ \frac{1}{cm^{3} \cdot eV} \right]
$$
Where $\frac{dN(E)}{dE}$ is the number of energy states $N(E)$ within an energy range $dE$.

We can find $N(E)$ geometrically reasoning on the following picture.
![[Screenshot_20241013_163231.png]]
This type of representation is in the space of $k$ that is linked with the momentum by $p = \hbar k$ ([[DOUBLE SLIT EXPERIMENT AND DE BROGLIE WAVELENGTH|de Broglie relations]])
Every point in this space represent a possible state possibly occupied by two electrons, one with spin up and the other with spin down. 
Since $k$ and $E$ are related by $(2)$ we can find first $N(k)$ and then obtain $N(E)$. 
$$
k = \sqrt{ \frac{2mE}{\hbar^{2}} } \tag{3}
$$

$N(E)$ can be calculated as the volume of a sphere of radius $k$ divided by the volume occupied by one energy state (the highlighted cube) :

$$
\begin{align}
N(k) &= \overset{ \substack{spins \\ \downarrow} }{ 2 } \frac{4/3 \pi k^{3}}{(2 \pi)^{3}/V} \\ 
N(E) &\overset{ (3) }{ = } \frac{8/3 \pi \left( \frac{2mE}{\hbar^{2}} \right)^{3/2}}{8 \pi^{3}/V} \\ 
& = \frac{V}{3 \pi^{2}} \left( \frac{2m}{\hbar^{2}} \right) ^{3/2} E ^{3/2} 
\end{align}
$$

From which we can obtain 

$$
\displaylines{
D(E) = \frac{1}{\cancel{ V }} \frac{\cancel{ V }}{\cancel{3} \pi^{2}} \left( \frac{2m}{\hbar^{2}} \right)^{3/2} \frac{\cancel{3}}{2} \sqrt{ E } \\\\

{\color{red} D(E) = \frac{1}{2 \pi^{2}} \left( \frac{2m}{\hbar^{2}} \right)^{3/2} \sqrt{ E }}  \quad \propto \sqrt{ E }
}
$$
![[Screenshot_20241013_164205.png]]
At **0 K**, all electrons occupy energy states below or equal to the **Fermi energy** $E_F$. This means that the lowest available energy states are filled, with the Fermi energy marking the highest energy level that is occupied by an electron.

Additionally, as energy increases, the **density of states** function $D(E)$ tells us that the number of available states increases. This occurs because, with increasing energy, there are more states that correspond to the same energy value but have different quantum numbers (or wavevectors) due to the system's dimensionality. These states are said to be **degenerate**, meaning that multiple quantum states have the same energy. However, they differ in their wavefunctions, typically in their spatial configurations or directions of momentum.

In other words, as energy grows, more degenerate states exist at higher energy levels, meaning the number of states with the same energy (but different wavefunctions) also increases. This is a key feature in three-dimensional systems, where higher energy states correspond to larger volumes in momentum space, allowing for more possible wavefunctions with the same energy.

### Fermi-Dirac Distribution
The Fermi-Dirac distribution is explained in [[EQUILIBRIUM FREE CHARGE CONCENTRATION|this note]].


## Limits of the Model
The **Fermi-Dirac distribution** is based on the assumption that energy states are spread continuously, which is generally valid for **metals**, where the available energy levels near the Fermi energy appear almost continuous due to the large number of closely spaced states. In metals, the conduction band is partially filled, allowing electrons to freely move and occupy states above the Fermi level.

However, this assumption breaks down for **semiconductors** and **insulators**. In these materials, there is a distinct **energy gap** (band gap) between the valence band (where electrons are bound to atoms) and the conduction band (where electrons are free to move). Within this energy gap, no available states exist for electrons, meaning they cannot occupy energies within this range without sufficient external excitation, such as thermal or optical energy.

As a result, the **Fermi-Dirac distribution** inadequately describes the behavior of semiconductors and insulators, because it does not account for the presence of this band gap, which significantly alters the distribution of available energy states and the occupation probabilities in these materials.

