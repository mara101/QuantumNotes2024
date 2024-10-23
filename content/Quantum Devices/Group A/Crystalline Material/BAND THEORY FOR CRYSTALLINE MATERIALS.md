Band theory in crystalline materials provides a foundational framework for understanding how electrons behave in solids. This theory explains the differences between conductors, semiconductors, and insulators based on the structure of energy bands formed in crystals.
In a single atom, electrons occupy specific, quantized energy levels. However, in a crystal, where many atoms are regularly arranged in a lattice, these atomic energy levels interact due to the influence of neighboring atoms. This interaction results in the splitting of energy levels into nearly continuous ranges called **energy bands**.

![[Screenshot_20241005_101501.png]]
![[Screenshot_20241005_101657.png]]![[Screenshot_20241005_101725.png]]
#### Formation of Energy Bands

In a crystalline material, when atoms are brought close together, the outermost electrons (valence electrons) of the atoms interact with those of neighboring atoms. Quantum mechanically, the energy levels of each atom split into closely spaced levels, forming a continuous range of allowed energies called a band.

The lower energy band is known as the **valence band**, where electrons are bound to atoms, and the higher energy band is called the **conduction band**, where electrons are free to move throughout the material. These two bands are separated by a region called the **band gap**, where no electron states exist.

The size of the band gap determines the electrical properties of the material:

- **Conductors** have overlapping valence and conduction bands, allowing free movement of electrons and thus high conductivity.
- **Semiconductors** have a small band gap, allowing limited electron movement from the valence to the conduction band when energy (e.g., thermal or light energy) is applied.
- **Insulators** have a large band gap, making it difficult for electrons to move from the valence band to the conduction band, resulting in very low conductivity.

#### Quantum Mechanics and Crystallinity

In a crystalline material, the regular periodic arrangement of atoms creates a periodic potential. This periodic potential allows for the exact solution of the Schrödinger equation, which describes the quantum behavior of particles. Solving this equation for the periodic potential leads to the formation of energy bands.

In non-crystalline (amorphous) materials, the lack of periodicity prevents the formation of well-defined energy bands. Thus, band theory applies strictly to crystalline materials.

#### Valence and Conduction Bands

Electrons in the **valence band** are involved in chemical bonding and are bound to specific atoms, while electrons in the **conduction band** are free to move through the material and contribute to electrical conduction. The **band gap** is the energy difference between the top of the valence band and the bottom of the conduction band. The electrical properties of a material are largely determined by the size of this band gap.

For instance:

- **Metals** (conductors) have either overlapping valence and conduction bands or a partially filled conduction band, allowing electrons to move freely and conduct electricity.
- **Semiconductors** have a small band gap (typically around 1 eV), allowing some electrons to transition to the conduction band at room temperature.
- **Insulators** have a large band gap (several electron volts), making it difficult for electrons to transition to the conduction band under normal conditions.

#### Effective Mass and Carrier Mobility

Electrons in a crystal are influenced by the periodic potential of the crystal lattice. This interaction modifies their mass, introducing the concept of **effective mass**. The effective mass describes how electrons (or holes) respond to external forces (like electric fields) while moving through the crystal. This effective mass can differ from the electron's rest mass and is a key factor in determining how easily carriers (electrons and holes) can move within the material. Holes are just a position in the band where the electron is missing and for simplicity of the calculation is considered as a particle with a positive charge with absolute value equals to the charge of an electron.
![[Screenshot_20241005_104315.png]]
#### Elements of the IV Group

Crystals formed by elements of group IV (such as carbon, silicon, and germanium) are known for their **covalent bonds**, which play a critical role in their electrical properties. The study of group IV crystals, especially silicon, is foundational for understanding semiconductor behavior, particularly in microelectronics.

The **silicon crystal structure** is an example of a covalent crystal, with a **face-centered cubic unit cell**. The covalent bonds in these materials create a **tetrahedral spatial arrangement** of atoms, meaning each atom in the crystal is bonded to four nearest neighbors, forming a three-dimensional network.

In isolated atoms, electrons occupy discrete ss and pp orbitals. For group IV elements, each atom has four valence electrons—two in ss and two in pp orbitals. When atoms come together to form a crystal, these discrete energy levels interact and split into closely spaced levels, forming **energy bands**.

- At **large inter-atomic distances**, the s-orbitals have 2N states filled with 2N electrons, while the p-orbitals have 6N states but only 2N electrons. The energy levels remain discrete, like isolated atoms.
- As the atoms come **closer together**, the s-and p-orbitals **hybridize** into sp3 orbitals. Initially, the s and p bands merge, and at even smaller distances, they split into two bands: the **valence band** (VB) and the **conduction band** (CB), each containing 4N states. The valence band is almost fully occupied by electrons, while the conduction band remains mostly empty at low temperatures.

The **band gap** (Eg​) between the valence and conduction bands plays a critical role in determining the electrical behavior of the material. In the case of silicon, the band gap is around **1.124 eV** at room temperature. When sufficient energy is provided (e.g., through heat or light), electrons can be excited from the valence band to the conduction band, allowing them to move freely and contribute to electrical conduction.

The size of the band gap decreases with increasing atomic number. For example:

- **Carbon (diamond)** has a band gap of about **5.47 eV**, making it an excellent insulator.
- **Silicon** has a band gap of about **1.124 eV**, making it a semiconductor.
- **Germanium** has a smaller band gap of about **0.66 eV**, making it more conductive than silicon.

These variations in the band gap explain why carbon behaves as an insulator, while silicon and germanium are semiconductors.
![[Screenshot_20241005_110713.png]]

#### Band Gap and Material Properties

The size of the band gap not only affects whether a material is a conductor, semiconductor, or insulator, but it also influences the material's **temperature dependence** and **carrier concentration**. Materials with a small band gap, like germanium, have a higher carrier concentration at room temperature compared to those with a larger band gap, such as silicon or diamond. This explains the higher electrical conductivity of germanium compared to silicon.
In a pure crystal the number of holes in the valence band are equals to the number of free electrons in the conduction band.
$$ n = \frac{number.of.free.electrons}{volume} (cm^{-3})$$
$$  p = \frac{number.of.holes}{volume} (cm^{-3})$$
So in a pure crystal we have $p = n$. Those properties are also useful to describe the electric property of the material.
#### Band Occupation and Electrical Properties

The electrical properties of a crystal depend on the occupancy of its energy bands. A completely filled valence band does not allow electron movement, so no electrical conduction can occur in this state. For electrical conduction to happen, electrons must be able to move to the conduction band, which requires overcoming the energy gap.

At **absolute zero temperature (0 K)**, semiconductors and insulators have no free electrons in the conduction band, meaning they act as insulators. However, as the temperature increases, some electrons gain enough thermal energy to jump from the valence band to the conduction band, creating free electrons (in the conduction band) and holes (in the valence band), which allows for electrical conduction.

