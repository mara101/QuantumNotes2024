# Photoresist

A **photoresist** is a light-sensitive material used in photolithography and other lithographic processes to form a patterned coating on a substrate. The photoresist plays a crucial role in defining the areas of the wafer that will be exposed to subsequent etching, doping, or deposition steps. When exposed to light, the chemical structure of the photoresist changes, which allows selective removal of either the exposed or unexposed areas during development. 
The photoresist is created, for the most part, with those three different elements:
- *Inactive polymer chain* that is the compound that gives the photoresist his mechanical and adhesion properties
- *Photoactive compound* which is the compound that gave the photoresist the ability to change with light.
- *Solvent* which allows the photoresist to stay in liquid form so it can be applied on the substrate.
There are two possible types of photoresists: **positive-photoresists** and **negative-photoresist**.
## Positive-Photoresist

In a positive photoresists, the regions exposed to light become more soluble in the developer solution, allowing them to be removed. This means that the pattern created in the photoresist will match the pattern on the mask (i.e., the exposed areas on the mask correspond to the areas removed in the photoresist). The photoresist become more soluble because the light will break down the polymeric chains present in the photoresist.

## Negative-Photoresist

In negative photoresists, the regions exposed to light become less soluble in the developer solution due to cross-linking of the polymer chains. This means that the unexposed areas are washed away, while the exposed areas remain on the wafer, forming the desired pattern.

## Resolution Capabilities, Exposure Energy, Sensitivity and Contrast

The performance of lithographic techniques depends on several factors, including **resolution capabilities**, **exposure energy**, **sensitivity**, and **contrast**. Each of these elements contributes to the accuracy and efficiency of the pattern transfer process.
### Resolution Capabilities

Resolution in lithography refers to the smallest feature size that can be reliably patterned onto a wafer. As devices become smaller and more complex, the ability to define smaller features with higher precision becomes necessary. The resolution limit of a lithographic process is typically determined by the wavelength of light used during exposure and the numerical aperture (NA) of the projection system.

The **Rayleigh criterion** is often used to define resolution, which depends on the wavelength ($\lambda$) and the numerical aperture (NA) of the system:
$$R = \frac{k_1 \cdot \lambda}{NA}$$
Where $R$ is the minimum feature size, $k_1$ is a process constant (which can be reduced with process optimizations), and NA is the aperture of the projection system. Shorter wavelengths of light, such as deep ultraviolet (DUV) at 193 nm and extreme ultraviolet (EUV) at 13.5 nm, allow for finer resolution. For example, DUV lithography can achieve resolution down to 45 nm, while EUV systems, still under development for large-scale manufacturing, have the potential to pattern features smaller than 20 nm.

However, physical limits arise due to factors like **diffraction**, mask imperfections, and substrate interactions. 
### Exposure Energy

The **exposure energy** is the amount of energy delivered to the photoresist during the exposure step. This energy must be carefully controlled to ensure that the photoresist reacts appropriately. 
The choice of exposure energy is critical because too little energy can lead to incomplete exposure, while too much can overexpose the resist, affecting the fidelity of the pattern transfer.
![[Screenshot_20241010_113918.png]]
### Sensitivity

**Sensitivity** in lithography refers to the amount of exposure energy required to achieve a desired change in the photoresist. High-sensitivity resists require less energy to expose, making them faster but potentially more prone to noise or unintended exposure effects. Conversely, lower sensitivity resists may offer higher resolution and contrast but require longer exposure times.

The **dose-to-clear** or **clearing dose** is an important measure of sensitivity. It represents the minimum exposure energy needed to fully develop a large clear area of the photoresist. Higher sensitivity resists have a lower dose-to-clear value, meaning they require less exposure energy to achieve the same effect.
### Contrast

**Contrast** in a photoresist system refers to the difference in solubility between the exposed and unexposed areas of the resist. High-contrast resists provide a sharper delineation between these regions, leading to more precise patterns. The **contrast ratio** is often represented as the slope of the development rate curve (also known as the **H-D curve**, after Hurter and Driffield, who originally developed the concept for photographic film).
![[Screenshot_20241010_115008.png]]

The contrast can be expressed mathematically as:
$$\gamma = \frac{1}{\log_{10}\left(\frac{E_f}{E_i}\right)}$$
Where $\gamma$ is the contrast, $E_f$ is the final exposure energy that just clears the resist, and $E_i$ is the initial exposure energy where the resist begins to develop. High-contrast resists have steep slopes, meaning a small increase in exposure energy results in a significant difference in development between exposed and unexposed areas.
![[Screenshot_20241010_115155.png]]

# Exposure Sources
The choice of exposure source directly impacts the resolution, speed, and cost-effectiveness of the lithography process. Over time, exposure sources have evolved from ultraviolet (UV) lamps to more advanced systems like deep ultraviolet (DUV) and extreme ultraviolet (EUV) light sources, allowing smaller feature sizes and higher precision in patterning. Below are the key exposure sources used in lithography.
###  Ultraviolet (UV) Exposure Sources

Historically, UV light has been the most commonly used exposure source in lithography, especially for semiconductor manufacturing. The wavelength of the UV light determines the resolution of the lithographic process, with shorter wavelengths providing higher resolution. There are three primary categories of UV light used in photolithography:

- **G-line (436 nm)**: This wavelength was used in earlier generations of lithography for feature sizes down to about 1 micron. It is named after the specific spectral line emitted by mercury vapor lamps.
    
- **I-line (365 nm)**: A shorter wavelength than G-line, I-line lithography allows for finer resolution, enabling feature sizes in the range of 0.5 microns. It became a standard for several generations of semiconductor fabrication.
    
- **Deep Ultraviolet (DUV, 248 nm and 193 nm)**: DUV lithography uses excimer lasers (e.g., KrF at 248 nm and ArF at 193 nm) to achieve much higher resolution than traditional UV sources. With these shorter wavelengths, it is possible to achieve feature sizes of 0.13 microns and smaller. ArF lithography, in particular, has been widely adopted for advanced semiconductor manufacturing and is used in creating features smaller than 100 nm.
    
![[Screenshot_20241010_120500.png]]

#### Excimer Lasers

Excimer lasers are gas lasers that operate by using a combination of a noble gas (such as Krypton or Argon) and a halogen (such as Fluorine). These lasers are pulsed, emitting high-intensity ultraviolet light. The excimer lasers used in lithography, primarily KrF and ArF, have been instrumental in pushing feature sizes below the 100 nm threshold.

- **KrF (Krypton Fluoride) lasers at 248 nm**: Used in DUV lithography for resolutions down to about 0.25 microns. It has been the workhorse of semiconductor lithography for many years.
    
- **ArF (Argon Fluoride) lasers at 193 nm**: These lasers allow for even finer resolutions, down to 0.12 microns, and are currently the dominant source for advanced semiconductor nodes.
    
- **F2 (Fluorine) lasers at 157 nm**: Despite the potential for higher resolution, F2 lasers have not been widely adopted due to technical challenges, including finding suitable resists and optical components that can work effectively at this wavelength.
    

#### 3. **Extreme Ultraviolet (EUV) Lithography**

EUV lithography represents the next major advancement in exposure sources for semiconductor manufacturing. EUV light operates at a wavelength of **13.5 nm**, which allows for extremely fine resolution, enabling features smaller than 10 nm. EUV technology is quite different from UV and DUV lithography, as it requires the use of reflective optics and operates in a vacuum environment to prevent the absorption of the EUV light by air or other materials.

EUV light is generated by directing a high-energy infrared (IR) pulsed laser onto a droplet of molten tin, creating a plasma that emits EUV light. However, the complexity and cost of EUV systems are significant challenges. These systems require intricate mirrors with multiple layers to reflect the EUV light effectively since traditional lenses cannot be used.

![[Screenshot_20241010_121304.png]]
### Electron-Beam Lithography (E-Beam)

Unlike optical lithography, which uses light to expose the resist, electron-beam (e-beam) lithography uses a focused beam of electrons. E-beam lithography is a maskless process, meaning it does not require a photomask to transfer patterns. Instead, the electron beam directly writes the desired pattern onto the resist. This technique provides extremely high resolution, down to the nanometer scale, making it ideal for research, mask fabrication, and small-volume production.

One of the main drawbacks of e-beam lithography is its speed. Since it writes patterns directly, it is much slower than optical lithography, which can expose entire areas at once. As a result, e-beam lithography is not typically used for mass production but is invaluable for creating masks and for R&D purposes.
![[Screenshot_20241011_110422.png]]
