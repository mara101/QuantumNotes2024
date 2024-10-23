We will now analyze the example of the infinite square well. The infinite square well is an idealized example to prove the quantum behavior of the particle and to find a simple solution to the time-dependent Schrodinger equation. 
We begin with a particle trapped in a one dimensional region bounded by infinite potential walls:
![[Screenshot_20241006_101921.png|350]]
So the particle is bounded in the region $0<= x >=a$.
![[Screenshot_20241006_102150.png]]
Now that the particle is bounded in this region where $V(x)= 0$ we can write a simplified version of the [[STATIONARY SOLUTIONS AND TIME INDEPENDENT SCHRODINGER EQUATION|time-independent Schrodinger equation]] without the term accounting or the potential energy.
![[Screenshot_20241006_102838.png|350]]
Now we used this type of form with the $k$ therm because we obtained a differential-type equation that is easy to solve and corresponds to the differential equation for *the simple harmonic oscillator*. Then we express the solution of the equation.
![[Screenshot_20241006_103314.png]]
Now that we obtained the general solution for the wave function independent of time we can do furthers simplifications. As we said the particle is in a region where $V = 0$ and $V = \infty$ outside. So there is a forbidden region where the particle have zero probability to be there. so it must follow that $\psi(0) = 0$ and $\psi(a) = 0$ , those are called *boundaries conditions*. If then  $\psi(0) = 0$ it must follow that:
![[Screenshot_20241006_104440.png]]
Because $\psi(0) = 0$ the also B = 0. So we can rewrite the equation with only the term that is represented by the sine function.
![[Screenshot_20241006_104725.png]]
Then we consider that also $\psi(a) = 0$ and we try to find the value of the coefficient A. $$\psi(a) = Asin(k0)$$
But there are only two solutions to this type of equation. The first one is the solution $A = 0$. This type of solution yields the solution $\psi(x) = 0$ which although a correct solution for the Schrodinger equation does not have a physical meaning because it does not respect the [[WAVE FUNCTION AND IT'S STATISTICAL REPRESENTATION|normalization property]].

So the only possible solution is the following: ![[Screenshot_20241006_105727.png]]
That is a quite curious type of solution, because it tells us that there are only discrete type of energy levels in the infinite square well and does not give us information about the value of $A$
![[Screenshot_20241006_110236.png]]
![[Screenshot_20241006_110212.png]]
To find the value of A we have to take the wave function $\psi(x)$ we have just obtained and normalize it.
![[Screenshot_20241006_110522.png]] 
So then we obtain our time-independent solution:
![[Screenshot_20241006_112733.png]]

Note that we cannot have a solution where $E = 0$, the minimum energy state we can obtain in this example is the energy given by the solution $\psi_1(x)$ that is called *ground state* whereas the others states are called *exited states*.
Now those collection of wave functions that we have obtained have different interesting properties.

- They are alternatively *even* and *odd*. That means that the wave function will have probability holes in respects to the center of the hole that depend on $n$. In particular ${number.of.probability.holes} = n-1$
-  The possible solutions are *mutually orthogonal* between them. That means that their [[CONNECTIONS WITH LINEAR ALGEBRA AND HILBERT SPACE|inner product]] is null if $n$ is not equal to $m$.
	![[Screenshot_20241006_113838.png]]
	That means that they form an orthonormal basis to express other types of wave functions.
-  They are *complete*, in the sense that any other function, f (x), can be
	expressed as a linear combination of them:
	![[Screenshot_20241006_114447.png]]
	Now completeness is a strong concept and a mess to prove so we will be good physicist and give it for a fact :)

The [[STATIONARY SOLUTIONS AND TIME INDEPENDENT SCHRODINGER EQUATION|stationary states]] of the infinite square well can be then expressed as such:
![[Screenshot_20241006_120653.png]]
Then as we have also expressed [[STATIONARY SOLUTIONS AND TIME INDEPENDENT SCHRODINGER EQUATION|here]]. The time-dependent Schrodinger equation can be expressed as a linear combination of stationary states:
![[Screenshot_20241006_120857.png]]
Then the coefficient $c_n$ can be found using the [[LINKS BETWEEN FOURIER SERIES AND THE SCHRODINGER EQUATION|Fourier trick]].
