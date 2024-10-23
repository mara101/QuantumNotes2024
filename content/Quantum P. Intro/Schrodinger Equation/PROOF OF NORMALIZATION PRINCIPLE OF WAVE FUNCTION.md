
## Normalization Condition

In quantum mechanics, the wave function $\psi(x, t)$ represents the state of a particle. The square modulus of the wave function, $|\psi(x, t)|^2$, gives the probability density of finding the particle at position $x$ at time $t$. This must integrate to 1 over all space, meaning that the total probability of finding the particle somewhere is 1. This is known as the **normalization condition**:

$$
\int_{-\infty}^{\infty} |\psi(x, t)|^2 dx = 1
$$

Our goal is to prove that if the wave function is normalized at $t = 0$, it remains normalized for all future times.

## Time Derivative of the Normalization Condition

To show that the normalization condition is preserved over time, we need to compute the time derivative of the integral and show that it equals zero:

$$
\frac{d}{dt} \int_{-\infty}^{\infty} |\psi(x, t)|^2 dx = 0
$$

### Step 1: Differentiate the Integral with Respect to Time

Start by differentiating the normalization condition:

$$
\frac{d}{dt} \int_{-\infty}^{\infty} |\psi(x, t)|^2 dx = \int_{-\infty}^{\infty} \frac{\partial}{\partial t} |\psi(x, t)|^2 dx
$$

This changes the total derivative to a partial derivative since the integrand depends on both $x$ and $t$.

### Step 2: Apply the Product Rule to $|\psi(x, t)|^2$

Since $|\psi(x, t)|^2 = \psi^*(x, t) \psi(x, t)$, we use the product rule to differentiate:

$$
\frac{\partial}{\partial t} |\psi(x, t)|^2 = \psi^*(x, t) \frac{\partial \psi(x, t)}{\partial t} + \frac{\partial \psi^*(x, t)}{\partial t} \psi(x, t)
$$

### Step 3: Substitute the Schrödinger Equation

Using the time-dependent Schrödinger equation:

$$
i\hbar \frac{\partial \psi(x, t)}{\partial t} = -\frac{\hbar^2}{2m} \frac{\partial^2 \psi(x, t)}{\partial x^2} + V(x, t) \psi(x, t)
$$

Solve for $\frac{\partial \psi}{\partial t}$:

$$
\frac{\partial \psi(x, t)}{\partial t} = \frac{i\hbar}{2m} \frac{\partial^2 \psi(x, t)}{\partial x^2} - \frac{i}{\hbar} V(x, t) \psi(x, t)
$$

Similarly, for the complex conjugate $\psi^*$:

$$
\frac{\partial \psi^*(x, t)}{\partial t} = -\frac{i\hbar}{2m} \frac{\partial^2 \psi^*(x, t)}{\partial x^2} + \frac{i}{\hbar} V(x, t) \psi^*(x, t)
$$

### Step 4: Substitute into the Time Derivative of $|\psi(x, t)|^2$

Substitute these expressions back into the time derivative of $|\psi(x, t)|^2$:

$$
\frac{\partial}{\partial t} |\psi(x, t)|^2 = \psi^* \left( \frac{i\hbar}{2m} \frac{\partial^2 \psi}{\partial x^2} - \frac{i}{\hbar} V(x, t) \psi \right) + \left( -\frac{i\hbar}{2m} \frac{\partial^2 \psi^*}{\partial x^2} + \frac{i}{\hbar} V(x, t) \psi^* \right) \psi
$$

Simplify:

$$
\frac{\partial}{\partial t} |\psi(x, t)|^2 = \frac{i\hbar}{2m} \left( \psi^* \frac{\partial^2 \psi}{\partial x^2} - \frac{\partial^2 \psi^*}{\partial x^2} \psi \right)
$$

### Step 5: Recognize a Total Derivative

The expression inside the parentheses is a total derivative with respect to $x$:

$$
\frac{\partial}{\partial t} |\psi(x, t)|^2 = \frac{\partial}{\partial x} \left( \frac{i\hbar}{2m} \left( \psi^* \frac{\partial \psi}{\partial x} - \frac{\partial \psi^*}{\partial x} \psi \right) \right)
$$

### Step 6: Integrate Over All Space

Now, substitute this result back into the integral:

$$
\frac{d}{dt} \int_{-\infty}^{\infty} |\psi(x, t)|^2 dx = \int_{-\infty}^{\infty} \frac{\partial}{\partial x} \left( \frac{i\hbar}{2m} \left( \psi^* \frac{\partial \psi}{\partial x} - \frac{\partial \psi^*}{\partial x} \psi \right) \right) dx
$$

By the **fundamental theorem of calculus**, the integral of a total derivative over the entire real line is equal to the values of the integrand at the boundaries, $x = \pm \infty$:

$$
\int_{-\infty}^{\infty} \frac{\partial}{\partial x} \left( \frac{i\hbar}{2m} \left( \psi^* \frac{\partial \psi}{\partial x} - \frac{\partial \psi^*}{\partial x} \psi \right) \right) dx = \left[ \frac{i\hbar}{2m} \left( \psi^* \frac{\partial \psi}{\partial x} - \frac{\partial \psi^*}{\partial x} \psi \right) \right]_{-\infty}^{\infty}
$$

### Step 7: Apply Boundary Conditions

For a normalizable wave function, $\psi(x, t)$ must go to zero as $x \to \pm \infty$, and so must its derivatives. Therefore, at the boundaries $x = \pm \infty$:

$$
\psi^*(x, t) \frac{\partial \psi(x, t)}{\partial x} - \frac{\partial \psi^*(x, t)}{\partial x} \psi(x, t) \to 0
$$

Thus, the boundary term vanishes:

$$
\left[ \frac{i\hbar}{2m} \left( \psi^* \frac{\partial \psi}{\partial x} - \frac{\partial \psi^*}{\partial x} \psi \right) \right]_{-\infty}^{\infty} = 0
$$

### Step 8: Conclusion

Since the boundary terms vanish, we conclude that:

$$
\frac{d}{dt} \int_{-\infty}^{\infty} |\psi(x, t)|^2 dx = 0
$$

Therefore, if the wave function is normalized at $t = 0$, it remains normalized for all future times.

This completes the proof that the normalization of the wave function is preserved under time evolution according to the Schrödinger equation.


#### Flashcards
Make the proof of the normalization principle of wave function related to Schrodinger equation::[[PROOF OF NORMALIZATION PRINCIPLE OF WAVE FUNCTION]]