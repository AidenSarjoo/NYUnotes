This is based off the course by Vikram Duvvuri at NYU Tandon, and borrows his explanations, problems, and material. 

Consult the textbook

# Simple Harmonic Motion

### variables:
- $\text{frequency} : f : [f] = HZ \text{ or } s^{-1}$
- $\text{period} : T : [T] = s$
- $\text{angular frequency} : \omega : [\omega] = HZ$
- $\text{phase constant} : \phi_0$

### equations:
- $f = \frac{1}{T} = \frac{1}{2\pi}\sqrt{\frac{k}{m}}$  
- $\omega = 2\pi f$
- $x(t) = A\cos(\omega t + \phi_0)$
- $v_{max}=\omega A$
- $v_{x}(t) = sin(\omega t + \phi_0)$

Oscillatory motion describes repetitive motion about an equilibrium point. Simple Harmonic Motion (SHM) is a type of oscillatory motion where the position and velocity are sinusoidal.

Recall frequency $f$ and period $T$ have an inverse relationship, so:
$f = \frac{1}{T}$

## The Phase Constant 
The phase constant $\phi_{0}$ accounts for the offset of SHM, like if the motion does not begin at rest $x = A$, thus augmenting our original equation to:
$x(t) = A\cos(\omega t + \phi_0)$

Thus, we can calculate the phase constant as:
$\phi_{0} = \arccos\left(\frac{x(t)}{A}\right) - \omega t$  