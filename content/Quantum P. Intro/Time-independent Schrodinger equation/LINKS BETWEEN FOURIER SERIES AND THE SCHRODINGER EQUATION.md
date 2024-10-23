
The Fourier series and Fourier transform play a significant role in quantum mechanics, particularly in solving the Schrödinger equation. These mathematical tools allow us to decompose complex wavefunctions into simpler components, helping us understand their behavior in both time and space.
Also you may want to reference those notes: [[THE FOURIER SERIES AND TRANSFORM|Fourier series and transform]]/[[INTERPRETATION OF WAVE FUNCTION AND IT'S FOURIER TRANSFORM|Interpretation of the wave function and the Fourier transform of the function]].
## The Link Between Fourier Series and the Schrodinger Equation
In quantum mechanics, wavefunctions can be expressed as linear combinations of basis functions. For a particle in a **box** (i.e., an infinite square well), the basis functions are sine and cosine waves, which correspond to standing waves within the box. These wave-forms are solutions to the time-independent Schrödinger equation in this confined system. The idea of expanding a function in terms of sines and cosines is rooted in **Fourier series**.

The Fourier series expansion of a function $f(x)$ over a finite interval $[0, a]$ is given by:

$$
f(x) = \sum_{n=1}^{\infty} c_n \sin \left( \frac{n\pi x}{a} \right),
$$

where $c_n$ are the Fourier coefficients that determine the contribution of each sine wave to the overall function.

In the context of quantum mechanics, the **Fourier series** allows us to represent an arbitrary initial wave function $\psi(x, 0)$ as a sum of stationary states, which are solutions to the time-independent Schrödinger equation.

## Completeness and Orthogonality
The sine functions used in Fourier series expansions are **orthogonal**. This means that for different values of $n$, the integrals of the products of the sine functions over the interval are zero unless they have the same index:

$$
\int_0^a \sin\left( \frac{n\pi x}{a} \right) \sin\left( \frac{m\pi x}{a} \right) dx = 0 \quad \text{for} \quad n \neq m.
$$

The **orthogonality** of these functions is crucial in quantum mechanics because it allows us to decompose complex wavefunctions into independent components that don’t interfere with each other. This property ensures that each quantum state (represented by a sine function) contributes separately to the total wavefunction.

## Fourier Transform and Wavefunctions
In quantum mechanics, particularly for free particles or systems without spatial boundaries, the Fourier **transform** is a more general tool than the Fourier series. The Fourier transform allows us to decompose wavefunctions into a continuous spectrum of plane waves (rather than a discrete set of standing waves as in the Fourier series). For example, a free particle wave packet can be expressed as:

$$
\psi(x, t) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \phi(k) e^{i(kx - \frac{\hbar k^2}{2m} t)} dk,
$$

where $\phi(k)$ is the Fourier transform of the initial wavefunction $\psi(x, 0)$.

This equation shows that any wave function can be represented as an integral of plane waves $e^{ikx}$, each with a different wave number $k$. The distribution of these plane waves is given by $\phi(k)$, which is found through the Fourier transform of the initial wavefunction:

$$
\phi(k) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \psi(x, 0) e^{-ikx} dx.
$$

This approach is particularly useful for describing free particles, where the Schrödinger equation does not have bound states, and the energy spectrum is continuous.

## Fourier's Trick in Quantum Mechanics
In solving quantum mechanical problems, we often employ **Fourier's trick**, which leverages the orthogonality of sine and cosine functions to calculate the coefficients in the expansion of a wavefunction. For example, given an initial wavefunction $\psi(x, 0)$, we can find the coefficients $c_n$ in its Fourier expansion using:

$$
c_n = \frac{2}{a} \int_0^a \psi(x, 0) \sin\left( \frac{n\pi x}{a} \right) dx.
$$

This allows us to express the wavefunction as a sum of stationary states.

