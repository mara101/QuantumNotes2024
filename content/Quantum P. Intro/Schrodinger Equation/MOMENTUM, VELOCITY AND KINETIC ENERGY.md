Now we have to talk about velocity. But first of all what the hell is even velocity when we can't even determinate precisely the position of a particle?
At this point we have the definition of expected value on the position of x which is $$\langle x \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \, x \, \psi(x, t) \, dx
$$
At this point we can define de velocity as $\frac{d \langle x \rangle}{dt} = \langle v \rangle$. Of course this type of definition of velocity is not our usual concept of velocity but rather the velocity of the variation of the expectation value of x when the wave function change during time.
From that notion then we can consider what is the meaning of momentum in quantum mechanics considering the [[SCHRODINGER EQUATION|Schrodinger equation]].

We start by considering the definition that we have just given:

$$
\frac{d \langle x \rangle}{dt} = \frac{d}{dt} \int_{-\infty}^{\infty} \psi^*(x, t) \, x \, \psi(x, t) \, dx
$$
Then we move the derivative in the integral(transforming the integral in a partial integral) and we proceed with the derivation:

$$
\frac{d \langle x \rangle}{dt} = \int_{-\infty}^{\infty} \left( \frac{\partial \psi^*(x, t)}{\partial t} \, x \, \psi(x, t) + \psi^*(x, t) \, x \, \frac{\partial \psi(x, t)}{\partial t} \right) dx
$$

Now we consider the time-dependent Schrodinger equation and transform it in a way that can be used later one to obtain a new definition of the derivative of time of $\psi$ and $\psi*$ :

$$
\frac{\partial \psi(x, t)}{\partial t} = \frac{i\hbar}{2m} \frac{\partial^2 \psi(x, t)}{\partial x^2} - \frac{i}{\hbar} V(x) \psi(x, t)
$$

$$
\frac{\partial \psi^*(x, t)}{\partial t} = -\frac{i\hbar}{2m} \frac{\partial^2 \psi^*(x, t)}{\partial x^2} + \frac{i}{\hbar} V(x) \psi^*(x, t)
$$

Substitute what we have just found in the integral(Note that the terms that contains the potential energy just cancels out):

$$
\frac{d}{dt} \langle x \rangle = \int_{-\infty}^{\infty} \left( \frac{i\hbar}{2m} \frac{\partial^2 \psi^*(x, t)}{\partial x^2} \, x \, \psi(x, t) - \frac{i\hbar}{2m} \psi^*(x, t) \, x \, \frac{\partial^2 \psi(x, t)}{\partial x^2} \right) dx
$$

Now we apply to the previous integral the integration by part and we obtain:

$$
\frac{d \langle x \rangle}{dt} = \frac{i\hbar}{m} \int_{-\infty}^{\infty} \psi^*(x, t) \frac{\partial \psi(x, t)}{\partial x} \, dx
$$

The result we obtain we interpret as:

$$
\frac{d \langle x \rangle}{dt} = \langle v \rangle = \frac{i\hbar}{m} \int_{-\infty}^{\infty} \psi^*(x, t) \frac{\partial \psi(x, t)}{\partial x} \, dx
$$
So what we have found is not the velocity itself but the expected value of velocity for the solution of the Schrodinger equation.
Now that we have velocity we may want to express another expected physical property which is momentum that is expressed simply as $p = mv$. And int the case for his expected value we can express it as:

$$ \langle p \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \left( -i\hbar \frac{\partial}{\partial x} \right) \psi(x, t) \, dx $$
Note the form we put that expression. We isolated what is called the *operator* of the physical observable. 
Every physical observable in quantum mechanics has it's own operator which is no more a number but rather something else(we will see it later). Those are some example of operators we have just seen or can easily derive: 
$$
\langle x \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \, \hat{x} \, \psi(x, t) \, dx
$$

So $\hat{x} = x$ is the operator.
The momentum operator in the position representation is:
$$
\hat{p} = -i\hbar \frac{\partial}{\partial x}
$$
The expectation value of momentum is:
$$
\langle p \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \, \hat{p} \, \psi(x, t) \, dx
$$

Substituting the operator $\hat{p}$:

$$
\langle p \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \left( -i\hbar \frac{\partial}{\partial x} \right) \psi(x, t) \, dx
$$

The kinetic energy operator is related to the momentum operator. The classical kinetic energy is $T = \frac{p^2}{2m}$, and in quantum mechanics, the kinetic energy operator is:

$$
\hat{T} = \frac{\hat{p}^2}{2m} = -\frac{\hbar^2}{2m} \frac{\partial^2}{\partial x^2}
$$

The expectation value of the kinetic energy is:

$$
\langle T \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \, \hat{T} \, \psi(x, t) \, dx
$$

Substitute the kinetic energy operator:

$$
\langle T \rangle = \int_{-\infty}^{\infty} \psi^*(x, t) \left( -\frac{\hbar^2}{2m} \frac{\partial^2}{\partial x^2} \right) \psi(x, t) \, dx
$$
