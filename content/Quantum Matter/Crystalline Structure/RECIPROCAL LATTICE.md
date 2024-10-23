The **reciprocal lattice**, is a key concept in the study of crystal structures. It is a lattice in Fourier space that is mathematically constructed from the [[BRAVAIS LATTICE AND CRYSTAL STRUCTURES|direct Bravais Lattice]]. While the Bravais lattice describes the periodicity in real space, the reciprocal lattice is essential in understanding the periodicity in momentum space, such as for diffraction and electronic band structures.

The reciprocal lattice originates from mathematical transformations applied to the Bravais lattice. This process is crucial because it allows us to delve into reciprocal space, where we gain a clearer and more insightful understanding of various physical properties inherent to crystals.

Let's start with a Bravais lattice:

$$ \mathbf{R}_n = n_1 \mathbf{a}_1 + n_2 \mathbf{a}_2 + n_3 \mathbf{a}_3 $$

where $n_1, n_2, n_3 = 0, \pm 1, \pm 2, \ldots$

We define the **reciprocal lattice** $\mathbf{G}$ such as:

$$ \mathbf{G} \cdot \mathbf{R}_n = 2m\pi \quad \text{where} \quad m = 0, \pm 1, \pm 2, \ldots $$

Note that the number of $\mathbf{G}$ vectors is infinite and that, since $\mathbf{R}_n$ is in meters $[m]$, $\mathbf{G}$ is $[m]^{-1}$, which is a reciprocal space.

We need to find a base for $\mathbf{G}$ in the reciprocal space that satisfies the following condition:

$$ \mathbf{a}_i \cdot \mathbf{g}_j = 2\pi \delta_{ij} \quad \delta_{ij} = \begin{cases} 
1 & i = j \\ 
0 & i \neq j 
\end{cases} $$

where $\mathbf{g}_j$ are the base vectors in the reciprocal space and $\mathbf{a}_i$ are the base vectors in the direct space.

Since we can find $\mathbf{g}_1, \mathbf{g}_2, \mathbf{g}_3$ given $\mathbf{a}_1, \mathbf{a}_2, \mathbf{a}_3$, we can write:

$$ \mathbf{G} = h \mathbf{g}_1 + k \mathbf{g}_2 + l \mathbf{g}_3 \quad \text{where} \quad h, k, l = 0, \pm 1, \pm 2, \ldots $$

which is again a Bravais lattice but in reciprocal space.

## Examples of Conversion from Direct Space to Reciprocal Space

The reciprocal lattice is constructed from the **direct lattice**, as shown in the figure. The direct lattice is represented with the basis vectors $\mathbf{a}_1$ and $\mathbf{a}_2$, and the reciprocal lattice is defined with vectors $\mathbf{g}_1$ and $\mathbf{g}_2$. The [[WIGNER-SEITZ CELL|Wigner-Seitz cells]] are drawn for both the direct and reciprocal lattices. The **Brillouin zone** is the Wigner-Seitz cell of the reciprocal lattice.
![[Screenshot_20241013_114834.png]]
### Reciprocal Lattice Construction:

Given the Bravais lattice in real space:

$$ \mathbf{R}_n = n_1 \mathbf{a}_1 + n_2 \mathbf{a}_2 $$

We can calculate the base vectors of the reciprocal space using the constraints:

1. $\mathbf{g}_1 \cdot \mathbf{a}_1 = 2\pi$
2. $\mathbf{g}_1 \cdot \mathbf{a}_2 = 0$
   - This implies that $\mathbf{g}_1$ is perpendicular to $\mathbf{a}_2$.
3. $\mathbf{g}_2 \cdot \mathbf{a}_1 = 0$
   - This implies that $\mathbf{g}_2$ is perpendicular to $\mathbf{a}_1$.
4. $\mathbf{g}_2 \cdot \mathbf{a}_2 = 2\pi$

From these relations, we derive the reciprocal lattice vectors:

$$
\mathbf{g}_1 = \frac{2\pi}{a_1 \cdot \cos(90^\circ)} = \frac{2\pi}{a_1}
$$
$$
\mathbf{g}_2 = \frac{2\pi}{a_2 \cdot \cos(90^\circ)} = \frac{2\pi}{a_2}
$$


