
# Ostrogradsky Works For:

$$L=\dddot{x}^2+\dddot{y}^2$$
$$L=\ddot{x}^2+\dddot{y}^3$$
- After fixing Issue 1, the code works for the following Lagrangian:
$$L=\dddot{x}^2+\ddot{y}^3+\ddot{z}^4$$
# Issues

1. For cases where finding $A$ results in multiple values, what do we do?
	- **Solution:** Find A and check if it has more than one element. If it does, take the first one (which will be the positive, real solution)
2. `Ostrogradsky()` does not handle dependent variables with highest order 0 in L correctly
	- **Solution:** Check for whether $N[k]=0$, if it is just set $A=X[k][1]$. Be sure to also set all $P_{x_k,0}=0$
3. Terms where the Nth derivative of two different variables are combined result in the Nth derivatives being displayed in the Hamiltonian. NOT CORRECT
	- **Potential Solution:** Solve A's as a system of equations, not as a singular equation because they may be coupled

