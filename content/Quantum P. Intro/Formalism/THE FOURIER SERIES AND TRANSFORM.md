
Fourier analysis provides powerful tools for decomposing functions into sinusoidal components. The **Fourier series** applies to periodic functions, while the **Fourier transform** generalizes this concept to non-periodic functions. Both are essential tools in physics, signal processing, and quantum mechanics.
## Fourier Series
The **Fourier series** is used to represent a periodic function as a sum of sine and cosine terms (or equivalently, complex exponentials). A periodic function $f(x)$ with period $T$ can be expressed as a Fourier series:

$$
f(x) = \sum_{n=-\infty}^{\infty} c_n e^{i n \omega_0 x}
$$

where:
- $c_n$ are the Fourier coefficients,
- $\omega_0 = \frac{2\pi}{T}$ is the fundamental frequency.

### Fourier Coefficients

The Fourier coefficients $c_n$ are calculated by projecting the function onto the complex exponential basis:

$$
c_n = \frac{1}{T} \int_{0}^{T} f(x) e^{-i n \omega_0 x} \, dx
$$

This gives the weight of each frequency component in the Fourier series.
### Example of a Fourier Series

For a square wave function, the Fourier series consists of only odd harmonics (terms involving odd multiples of the fundamental frequency). The more terms in the series, the better the approximation of the function.

## Fourier Transform

The **Fourier transform** generalizes the idea of the Fourier series to non-periodic functions. Instead of a sum over discrete frequencies, the Fourier transform represents a function as an integral over continuous frequencies.

For a function $f(x)$ defined over all real numbers, the Fourier transform $\hat{f}(k)$ is given by:

$$
\hat{f}(k) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} f(x) e^{-ikx} \, dx
$$

where:
- $\hat{f}(k)$ is the Fourier transform of $f(x)$,
- $k$ is the frequency variable (or wave number in physical applications).

### Physical Interpretation

The Fourier transform $\hat{f}(k)$ represents the function $f(x)$ in the **frequency domain**. The square of the magnitude $|\hat{f}(k)|^2$ gives the **power spectrum**, or how much of each frequency component is present in the original function $f(x)$.

## Inverse Fourier Transform

The **inverse Fourier transform** allows you to reconstruct the original function $f(x)$ from its Fourier transform $\hat{f}(k)$:

$$
f(x) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \hat{f}(k) e^{ikx} \, dk
$$

This integral effectively sums up all the frequency components, each multiplied by their corresponding exponential factor $e^{ikx}$.

### Relationship Between Direct and Inverse Transforms

The Fourier transform and its inverse form a pair of operations that allow for switching between time (or position) space and frequency space:
- The **Fourier transform** takes you from the time domain $f(x)$ to the frequency domain $\hat{f}(k)$.
- The **inverse Fourier transform** brings you back from the frequency domain to the time domain.

## Fourier Transform vs. Fourier Series

### Fourier Series:
- Decomposes **periodic** functions into a sum of sine and cosine terms (discrete frequencies).
- Uses a sum over harmonics of a fundamental frequency.
- Applicable when the function is defined over a finite interval and repeats periodically.

### Fourier Transform:
- Decomposes **non-periodic** functions into continuous frequency components.
- Uses an integral to sum over all possible frequencies.
- Applicable when the function is defined over an infinite domain and is not periodic.

## 5. Properties of Fourier Transforms

1. **Linearity**:
   The Fourier transform of a sum of functions is the sum of their Fourier transforms:
   $$
   \mathcal{F}\{a f(x) + b g(x)\} = a \hat{f}(k) + b \hat{g}(k)
   $$

2. **Translation**:
   A shift in position results in a phase shift in the Fourier transform:
   $$
   \mathcal{F}\{f(x - x_0)\} = e^{-ikx_0} \hat{f}(k)
   $$

3. **Scaling**:
   If you scale the input function, the Fourier transform scales inversely:
   $$
   \mathcal{F}\{f(ax)\} = \frac{1}{|a|} \hat{f}\left(\frac{k}{a}\right)
   $$

4. **Convolution**:
   The Fourier transform of the convolution of two functions is the product of their Fourier transforms:
   $$
   \mathcal{F}\{f(x) * g(x)\} = \hat{f}(k) \hat{g}(k)
   $$

5. **Parseval’s Theorem**:
   The total energy in a function is preserved in its Fourier transform:
   $$
   \int_{-\infty}^{\infty} |f(x)|^2 \, dx = \int_{-\infty}^{\infty} |\hat{f}(k)|^2 \, dk
   $$
