This notes explain the various process of exposure of the substrate
### Exposure Tools

Lithography requires specific tools for exposing the wafer to light in order to transfer patterns from a mask. The exposure tools are responsible for projecting the image of the mask onto the wafer's surface, a critical process for defining the tiny features in micro- and nanofabrication.

#### Contact Exposure

In **contact exposure**, the mask is placed directly in contact with the wafer. This method allows for high resolution because there is no gap between the mask and the wafer, minimizing diffraction and other optical distortions. However, contact exposure also has significant drawbacks:

- The mask can become damaged after repeated contact with the wafer, reducing its longevity.
- Any particles trapped between the mask and the wafer can create defects in the pattern.

Despite these issues, contact exposure is still used in some research and development settings due to its simplicity and cost-effectiveness. It is particularly useful for small-scale or prototype fabrication where frequent mask replacement is acceptable.
![[Screenshot_20241011_112017.png]]
The parameter $b_{min}$​ represents the smallest width or spacing that can be printed or patterned onto a wafer with a given lithography setup.
#### Proximity Exposure

**Proximity exposure** is similar to contact exposure, but in this method, a small gap is maintained between the mask and the wafer, typically in the range of tens of micrometers. The presence of this gap helps to preserve the integrity of the mask by reducing the wear and tear that would occur with direct contact. However, this also introduces optical diffraction, which limits the resolution achievable with proximity exposure compared to contact exposure.
![[Screenshot_20241011_112625.png]]
In this case $b_{min}$ is greater that in the case of contact exposure because we are adding a term $s$ that represent the gap of the mask from the substrate.
#### Projection Exposure
![[Screenshot_20241011_113617.png]]
**Projection exposure** is the most widely used technique in modern semiconductor manufacturing. In this method, the mask image is projected onto the wafer through a complex optical system. The system can include lenses and mirrors to reduce or enlarge the image as needed, typically using a step-and-repeat process to cover the entire wafer surface. This is because lenses have a magnification value, for example 5x 4x or 10x. That means for example, that if we want to expose the substrate with a system that has a magnification constant of 10x that means that in a single exposure we covere $\frac{1}{100}th$ of the substrate and will have to do one hundreds exposures and that the mask must represent also $\frac{1}{100}th$ of the entire wafer. It also means that if the feature that you want to expose is larger than the 1% of the surface, you may need to use different masks to extend the same feature.

Projection exposure offers several advantages:

- Higher resolution is achievable due to the optical system, which reduces distortion and diffraction effects.
- The mask does not come into contact with the wafer, preserving its lifespan and reducing the risk of contamination.

Projection exposure is the basis for most modern photolithography systems used in high-volume semiconductor manufacturing, particularly for devices with sub-micrometer features. Also it is very expensive, about 150 millions for the entire system of lenses  :O
### Advanced Exposure Tools: Projection Steppers and Scanner

A **projection stepper** is a type of projection exposure tool that uses a step-and-repeat method to expose different areas of the wafer sequentially. The stepper moves the wafer in small increments (or steps) between exposures, allowing the entire wafer to be patterned using the same mask. The projection stepper is widely used for integrated circuit fabrication due to its ability to produce very fine patterns with high precision.

![[Screenshot_20241011_114908.png]]
A **scanner** is a more advanced version of a stepper, using a **step-and-scan** process rather than step-and-repeat. In a scanner:

- Both the mask (reticle) and the wafer move simultaneously during the exposure process. The mask is scanned across the exposure field in one direction, while the wafer moves in the opposite direction.
- This scanning process allows the projection system to expose a larger area of the wafer more efficiently.
- By continuously moving the mask and wafer, the scanner achieves greater precision and higher throughput compared to steppers.
Scanners allow for better focus control and are typically used in **deep ultraviolet (DUV)** lithography and **extreme ultraviolet (EUV)** lithography, where feature sizes are very small (down to 7 nm and below). This method is highly preferred in advanced semiconductor manufacturing due to its higher resolution and faster processing speed.
![[Screenshot_20241011_120127.png]]
### Front-Backside Alignment

In advanced lithography processes, it is often necessary to align patterns on both sides of the wafer. **Front-backside alignment** tools allow for precise alignment of patterns on the front and back of the wafer, ensuring that features on opposite sides of the wafer are correctly positioned relative to each other.

This alignment is particularly important in complex devices such as microelectromechanical systems (MEMS), where components on both sides of the wafer must interact precisely. Achieving accurate alignment is a technical challenge, requiring highly precise optical systems and alignment marks on both sides of the wafer.
![[Screenshot_20241011_120317.png]]
![[Screenshot_20241011_120415.png]]

### Reflections and Standing Waves

One challenge encountered in photolithography is the formation of **reflections and standing waves** during exposure. These phenomena occur when light reflects off the substrate or underlying layers of the wafer, interfering with the light passing through the mask. The result can be the formation of standing waves, which create variations in the intensity of the light reaching the photoresist. These intensity variations can lead to uneven exposure of the resist, causing defects in the final pattern.

Various techniques are used to mitigate the effects of reflections and standing waves, including the use of anti-reflective coatings and optimizing the exposure conditions.
![[Screenshot_20241011_120658.png]]
![[Screenshot_20241011_120737.png]]
![[Screenshot_20241011_120810.png]]
