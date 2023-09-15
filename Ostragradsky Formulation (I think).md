
## Normal Conversion of Lagrangian to Hamiltonian

$$L=L(q,\dot{q},t)$$
let the conjugate momentum $p$ be given by $$p=\frac{dL}{d\dot{q}}$$
The Hamiltonian can be computed via 
$$H=p\dot{q}-L$$

## Generalization

Let the Lagrangian be given by 

$$L=L(q,\dot{q},\ddot{q},...,q^{(n)},t)$$
Let $q_1=q, q_2=\dot{q},q_3=\ddot{q}$, up to $q_{n}$. The conjugate momenta are given by
$$p_i=\sum\limits_{j=i}^{n}(-\frac{d}{dt})^{j-i}\frac{\partial L}{\partial q^{(j)}}$$

The Hamiltonian is then given by 
$$H=\sum\limits_{i=1}^n p_i\dot{q_i}-L$$
and the Hamilton Equations are given by $$\dot{q_i}=\frac{\partial H}{\partial p_i}$$ and $$\dot{p_i}=-\frac{\partial H}{\partial q_i}$$
### Multiple Dependent Variables

If your Lagrangian has multiple dependent variables (like x and y), simply add a summation term for each dependent variable

Label dependent variables $q^1,q^2,q^3,...,q^m$

Hamiltonian is given by

$$H=\sum\limits_{j=1}^m\sum\limits_{i=1}^n p_i^j \dot{q_i}^j - L$$