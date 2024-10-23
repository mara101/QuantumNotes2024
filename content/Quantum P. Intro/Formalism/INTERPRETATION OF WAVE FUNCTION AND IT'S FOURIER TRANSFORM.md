
When you perform a Fourier transform of a wave function $\psi(x)$ to obtain a wave function in momentum space (or wave number space, represented by $k$), the resulting function, typically denoted as $\tilde{\psi}(k)$, represents the **momentum distribution** of the quantum state.

## What the Fourier-Transformed Wave Function Represents

- In **position space**, $\psi(x)$ describes the probability amplitude of finding a particle at a particular position $x$.
- In **momentum space**, $\tilde{\psi}(k)$ (the Fourier transform of $\psi(x)$) describes the probability amplitude of finding the particle with a particular **wave number** $k$, which is related to the particle's momentum.

The relationship between wave number $k$ and momentum $p$ is given by:
$$
p = \hbar k
$$
where $\hbar$ is the reduced Planck constant. Thus, $\tilde{\psi}(k)$ can also be interpreted as the wave function in **momentum space**, which gives information about the momentum distribution of the particle.

## Physical Interpretation

- The square of the magnitude of $\tilde{\psi}(k)$, i.e., $|\tilde{\psi}(k)|^2$, gives the **probability density** of finding the particle with momentum $p = \hbar k$. This is analogous to how $|\psi(x)|^2$ in position space gives the probability density of finding the particle at position $x$.
  
  In summary:
  - $|\psi(x)|^2$ tells you **where** the particle is likely to be found (in position space).
  - $|\tilde{\psi}(k)|^2$ tells you **what momentum** (or wave number) the particle is likely to have (in momentum space).

## The Uncertainty Principle and Wave Packets

The relationship between $\psi(x)$ and $\tilde{\psi}(k)$ also highlights an important aspect of the **uncertainty principle**. If $\psi(x)$ is highly localized in position space, $\tilde{\psi}(k)$ will be more spread out in momentum space, and vice versa. This expresses the fact that the more precisely you know a particle's position, the less precisely you can know its momentum, and vice versa.

## Fourier Transform Formula

The Fourier transform of a wave function $\psi(x)$ in position space to momentum space is given by:
$$
\tilde{\psi}(k) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \psi(x) e^{-ikx} \, dx
$$

And the inverse Fourier transform, which allows you to retrieve the position-space wave function from the momentum-space wave function, is:
$$
\psi(x) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{\infty} \tilde{\psi}(k) e^{ikx} \, dk
$$
