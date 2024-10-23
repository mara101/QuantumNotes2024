The **Bravais lattice** is a set of discrete points in space arranged in a periodic pattern such that the environment around any point is identical to every other point. In other words, it is a mathematical construct that describes the repetitive, translational symmetry of a crystalline structure. Note that not every lattice is a Bravais lattice.

The formula for a **Bravais lattice** describes how any point in the lattice can be generated from a set of **primitive vectors**:
$$ R = n_1a_1 + n_2a_2 + n_3a_3$$
where the a's are *primitive vectors* that defines the simple cell and n are integers that defines the next cell.
A Bravais lattice must satisfy two key conditions:
1. **Translational Symmetry**: Translating the entire lattice by any lattice vector does not change the appearance of the lattice.
2. **Identical Environments**: Every point in the lattice has the same local environment as any other point.
Those are examples of Bravais lattice and normal lattice:
![[Screenshot_20241007_150434.png|400]]
![[Screenshot_20241007_150646.png]]
![[Screenshot_20241007_150705.png|400]]
The first an last immage represent types of Bravais lattice and the middle one is not one of them because id does not follow the property of identical environments seen before. Note that the choice of the base cell is not unique.
This is the definition of primitive cell:
- A **primitive cell** is the smallest volume in a crystal lattice that, when translated by all the lattice vectors of the Bravais lattice, fills the entire space without any gaps or overlaps. It contains exactly one lattice point and represents the fundamental building block of the crystal structure.

There are in total 14 types of Bravais lattice:

![[Screenshot_20241008_164602.png|400x400]]

## Crystal Structure
A crystal structure is the union of a lattice and a basis. We have already seen that a **lattice** is just a periodic disposition of points in space. 
The **basis** (or sometimes called a "base") is a set of atoms or molecules associated with each lattice point. This means that at every point of the lattice, you place a group of atoms in a specific arrangement. These atoms could be one, several, or even complex molecules.
This is an example in the case of a single atom base:
![[Screenshot_20241008_170346.png|400x200]]
This is the case for a multi-atom base:
![[Screenshot_20241008_170525.png|400]]
and this is the case for a complex molecule:
![[Screenshot_20241008_170846.png|400x250]]
The type of crystal structure that a material crystallize to depends on the nature of the chemical bonds between the atoms. Also in a natural process everything crystallize following a Bravais lattice. 

### Silicon Crystal Structure
The silicon crystal structure is an example of the **diamond cubic structure**, which is a type of **face-centered cubic (FCC)** arrangement. The structure of silicon is defined by the combination of a lattice and a basis.

The lattice in this case is face-centered cubic, meaning that silicon atoms are positioned at each corner of a cube and at the center of each face of the cube. However, this lattice alone doesn’t fully describe the silicon crystal. To complete the description, we must include the basis, which in the case of silicon consists of two atoms per lattice point.

The first atom in the basis is positioned at the lattice point itself. The second atom in the basis is located within the unit cell but is shifted from the first atom by a specific amount. This displacement is described using **fractional coordinates** relative to the unit cell dimensions. These fractional coordinates indicate how far the second atom is from the lattice point in terms of fractions of the unit cell’s edge lengths(int the case of the figure a). The fractional coordinates for silicon are (¼, ¼, ¼) because the second atom is displaced by a quarter of the distance along each axis relative to the first atom(if we consider the first atom placed in the coordinates (0,0,0)).
![[Screenshot_20241008_173525.png|400x300]]
This diamond structure, typical of silicon and other semiconductors, results from the combination of the FCC lattice with this two-atom basis. The arrangement provides a highly symmetrical and stable structure, which plays a critical role in silicon’s properties as a semiconductor material.


