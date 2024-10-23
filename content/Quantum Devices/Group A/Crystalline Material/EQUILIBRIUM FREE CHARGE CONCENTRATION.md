### Equilibrium Free Charge Concentrations

The **equilibrium free charge concentrations** in a semiconductor refer to the number of **free electrons** in the conduction band and **holes** in the valence band under **thermal equilibrium** conditions (i.e., when no external forces like electric fields are applied). The behavior of these charge carriers is governed by the material's temperature and the **Fermi-Dirac distribution** of energy levels.

#### **Electron and Hole Concentrations**

In a semiconductor, the concentration of **free electrons** in the conduction band ($n$) and **holes** in the valence band ($p$) can be expressed as functions of their respective **energy distribution functions**. These functions describe the probability that a given energy state in the conduction or valence band is occupied by a charge carrier.

The concentrations are calculated by integrating the product of two terms:
1. The **density of states** in the conduction band ($N_c$) for electrons or in the valence band ($N_v$) for holes, which describes how many energy states are available at each energy level.![[Screenshot_20241005_181407.png|400]]
![[Screenshot_20241005_151815.png]]
2. The **occupation probability**, given by the **Fermi-Dirac distribution function** $f(E)$, which indicates the likelihood that an energy state at a certain energy $E$ is occupied by an electron.

Thus, the electron concentration in the conduction band $n$ is:

$$
n = \int_{E_c}^{\infty} N_c(E) f(E) \, dE
$$

And the hole concentration in the valence band $p$ is:

$$
p = \int_{-\infty}^{E_v} N_v(E) [1 - f(E)] \, dE
$$

Where:
- $E_c$ is the energy level of the **conduction band minimum**,
- $E_v$ is the energy level of the **valence band maximum**,
- $f(E)$ is the **Fermi-Dirac distribution function**.

#### **Why We Integrate From $-\infty$ to $+\infty$**

The integrals for electron and hole concentrations run over the entire range of possible energy levels. For electrons in the conduction band, we integrate from the conduction band minimum $E_c$ to infinity, because the conduction band starts at $E_c$ and higher energy states are available above it.
For holes, we integrate from $-\infty$ to $E_v$ because the holes represent missing electrons in the valence band, and we must account for all possible states in the valence band, which extend to energies lower than $E_v$. The integral is from $-\infty$ because the energy levels below the valence band maximum could be occupied by electrons, thus contributing to the total hole concentration.

As energy increases far above the Fermi level ($E \gg E_F$), the exponential term 

$$
\exp\left(\frac{E - E_F}{k_B T}\right)
$$

grows very large, and the Fermi-Dirac distribution function approaches zero very quickly. This means that, even though the upper limit of the integral is infinity, the occupation probability $f(E)$ approaches zero fast enough that the integral converges and does not blow up to infinity.
#### **Fermi-Dirac Distribution and Carrier Probability**

At thermal equilibrium, the **Fermi-Dirac distribution** describes the probability that an electron occupies an energy state at a certain temperature $T$. It is given by:

$$
f(E) = \frac{1}{1 + \exp\left(\frac{E - E_F}{k_B T}\right)}
$$
![[Screenshot_20241005_143714.png]]
Where:
- $E_F$ is the **Fermi level**, which represents the energy at which the probability of occupation by an electron is 50%,
- $E$ is the energy of the electron,
- $k_B$ is **Boltzmann’s constant**,
- $T$ is the **absolute temperature**.

For holes, the probability of a state being occupied is the complement, $1 - f(E)$, since a hole represents the absence of an electron.

Note that in the Fermi-Dirac distribution we have a step function in case of T=0K. That means that the energy levels before $E_f$ are fully occupied by electrons and for energy levels over the Fermi Levels are fully empty.
Therefore we can provide a second physical meaning to the Fermi level: *the maximum energy an electron can occupy (at thermal equilibrium) at the absolute zero temperature*. Notice however that at 𝑇 = 300 K the transition, although not abrupt as at 𝑇 = 0 K, still is very steep. This means that at room temperature most of the electrons still occupy states with energy $𝐸 ≤ E_f$.

## Derivation of $n, p, N_v and N_c$

Now that we have defined what are we working with let's try to put in a more convenient form the values that we are trying to derive. Now we have $p$ and $n$ in that form:
![[Screenshot_20241005_152729.png|400]]
But this type of integral does not admit a solution. To deal with this we have to use the Fermi-Integral solution of order of 1/2 and solve ultimately with numerical methods. The Fermi-Integral form is:
![[Screenshot_20241005_153615.png]]
Then we express $n$ with this form:
![[Screenshot_20241005_181152.png]]
Then we solve the integral numerically and we obtain:
![[Screenshot_20241005_181553.png]]
Now that process will be also done for $p$:
![[Screenshot_20241005_182731.png|400]]
Now if we analyze the Fermi-Integral we can see that for values of x< 0 we can make an approximation with the exponential function that becomes better if the magnitude of x big enough. 
![[Screenshot_20241005_183313.png]]![[Screenshot_20241005_183508.png|400]] 
A check on the expressions that we obtained for $n$ and $p$ shows that the argument for $F_{\frac{1}{2}}(x)$ is negative when $E_f >= E_c$ for $n$ and $E_f <= E_v$ for $p$.
That means that if $E_f$ is placed in the forbidden region then $F_{\frac{1}{2}}(x)$ can be expressed as an exponential function. 
![[Screenshot_20241007_084016.png]]

A semiconductor where the Fermi energy level is placed in the middle of the forbidden band is called *non-degenerative*, otherwise if the level is near one of the two bands or even in one of those, the semiconductor is called *degenerative*.

## Intrinsic Fermi Level
In an *intrinsic semiconductor* (a semiconductor that has not been [[DOPING CHEMICAL INTERPRETATION|doped]]) we can assume that the the concentration of holes and electrons are the same and we can write:
![[Screenshot_20241007_085310.png]]Then we can express $E_{fi}$ in function of the other variables:
![[Screenshot_20241007_085513.png]]
But if we are considering an intrinsic semiconductor we can also assume that $N_c$ and $N_v$ have comparable values and so the logarithm goes to zero. So $E_{fi}$ becomes:
![[Screenshot_20241007_085803.png]]
So in an intrinsic semiconductor we can assume that the intrinsic Fermi energy level, that represent the Fermi level in the case for a non doped semiconductor, is placed around the center of the band gap.
## Shockley equations
The Shockley equations describe the relationship between carrier concentrations in semiconductors under thermal equilibrium. These equations are crucial for understanding the behavior of electron and hole populations in both intrinsic and extrinsic semiconductors. For a non-degenerate semiconductor, the Shockley relations can be written as:
![[Screenshot_20241007_091508.png]]where $E_{fi}$ is the intrinsic Fermi level that we have just seen, $n_i$ and $p_i$ are the intrinsic concentration of the non-doped non-degenerative semiconductor at thermal equilibrium. These equations indicate that the electron and hole concentrations are exponentially dependent on the difference between the Fermi level and the intrinsic Fermi level. For an n-type semiconductor, where the electron concentration is higher, the Fermi level moves towards the conduction band, while in p-type semiconductors, the Fermi level moves towards the valence band. The Shockley equations only hold under thermal equilibrium and in non-degenerate semiconductors​.
![[Screenshot_20241007_092140.png]]

## The Mass Action Law
The mass action law provides a fundamental relationship in semiconductors that relates the electron and hole concentrations at equilibrium. It states that for any non-degenerate semiconductor at thermal equilibrium, the product of the electron concentration n and the hole concentration pp is constant and equal to the square of the intrinsic carrier concentration:$$np = n_i^2$$
This relationship holds because increasing the concentration of one type of carrier (through doping or external conditions) will proportionally decrease the concentration of the opposite type to maintain the equilibrium product. In essence, electron and hole concentrations cannot be independently controlled in a semiconductor without affecting each other​​.

This law is particularly important in describing the behavior of extrinsic semiconductors, where doping changes the electron and hole concentrations. For example, in n-type materials, the electron concentration increases, leading to a corresponding decrease in the hole concentration to maintain the balance defined by the mass action law. Similarly, in p-type materials, hole concentration increases and electron concentration decreases.

