But now we must confront the question: How the hell we solve the Schrodinger equation for $\psi(x,t)$ given the potential $V$?
In this for simplicity we will consider only $V(x)$ which is independent form time. So how do we solve the [[SCHRODINGER EQUATION|Schrodinger equation]]?
![[Screenshot_20241002_111200.png]]
We start simply to trying to separate $\psi$ in a form that contains two separate functions, one that contains the position dependence and another that contains the time dependence.
![[Screenshot_20241002_111635.png]]
In order to construct a more general solution we have to solve two separate equations, one dependent on time and the other on position. This is the following procedure to separate them:
![[Screenshot_20241002_112001.png]]
We have just rewrote the Schrodinger equation with the separated single variable function. We used the following property of partial derivatives:
![[Screenshot_20241002_112137.png]]

Now that we obtained the Schrodinger equation in a more friendly form we can try to separate the two functions on the left and on the right.
![[Screenshot_20241002_113043.png]]
Now that we obtain that form we can notice a very important fact about this formula. The two ends *are always constants* otherwise if one of the two total values of the two ends changes with time or position this relationship between the function wouldn't add up.
So we can divide as we said previously the two function and solve them one at a time.
(The choice of $E$ as a constant will be more clear later).
![[Screenshot_20241002_113549.png]]

### Solution of the time dependent part of the wave function
This type of equation is very straightforward to solve. What is the only function that derived will give itself multiplied with a constant? Of course the exponential function. So the result of this equation will give:
![[Screenshot_20241002_114136.png]]


### Solution of the time-independent Schrodinger equation
With that type of solution I anticipate that we will find the *stationary solutions or stationary states* of the Schrodinger equation. Those type of waveform solution does depend on times but have special properties where the probability distribution *does not* depend on time and the energy for a stationary state is constant, also all the expectations values of any dynamical variable remains constant. This properties are truly remarkable because, as we will see, normal solutions could be expressed as linear combinations of stationary states.

- **Stationary states time independence**
	We will demonstrate the time time independence of the probability distribution of the wave function even if itself depends on time:
		![[Screenshot_20241002_120249 1.png]]
		![[Screenshot_20241002_120505.png]]
	Note that the time dependence of the wave function above becomes just a phase factor. Now considering a general operator $A$ we can demonstrate as we have just made it's independence of time. For the expectation value of an observable $A$ in a stationary state $\psi(x,t)$ is given by:
   $$
   \langle A \rangle = \int_{-\infty}^{\infty} \psi^*(x,t) \hat{A} \psi(x,t) \, dx
   $$
   Since $\psi(x,t) = \psi(x) e^{-iE_n t/\hbar}$, this phase factor does not affect the expectation value when calculating observable that only involve spatial operators, meaning that these expectation values will not depend on time. So $\langle A \rangle$ is constant
- **Stationary states possesses a definite total energy**
	In classical mechanics the total energy expression is called the **Hamiltonian**.
	![[Screenshot_20241002_184000.png]]
	Now in quantum mechanics this is an operator obtain by canonical substitution of p with $\hat{p} = -i\hbar \frac{\partial}{\partial x}$ obtaining the following Hamiltonian operator:
	![[Screenshot_20241002_184610.png]]
	And the expectation value of the total energy is equals to:
	![[Screenshot_20241002_184818.png]]
	 So we discovered that the expected value of the Hamiltonian operator gives back the total energy of the stationary solution, but we can also demonstrate that this type of value is the only possible value for the total energy of the stationary state.
	 If we consider this representation of the operator $H$ we can rewrite the Schrodinger equation in a new and more compact way:$$ \hat{H} \psi(x) = E \psi(x) $$
	 This is called **Time-independent Schrodinger equation** and it's very important because is the starting point to solve the time-dependent Schrodinger equations.
- **The general solution is the linear combination of separable solutions**
	Now this is maybe the most important property for the stationary states. As we are about to discover each time-dependent Schrodinger eq. solution will yield an infinite series of wave functions($\psi_1(x), \psi_2(x), \psi_3(x),...)$ , each of one representing a possible allowed energy $(E_1,E_2,E_3, ...)$. So every wave function represent a possible energy level. 
	
	![[Screenshot_20241002_191943.png]]
	

