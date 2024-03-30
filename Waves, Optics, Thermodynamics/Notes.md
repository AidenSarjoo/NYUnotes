This is based off the course by Vikram Duvvuri at NYU Tandon, and borrows his explanations, problems, and material. He is the best.

Consult the [[Giancoli.pdf|textbook]]  for in-depth explanations, and the phenomenal problem solutions by [Zhangjin Xu](https://www.youtube.com/channel/UCfMdyd8Q69Px3T0vaLEL6SA) on YouTube
# Syllabus:
- [[Waves, Optics, Thermodynamics/Notes#Simple Harmonic Motion|Simple Harmonic Motion (14.1 - 14.5)]]
	- [[Waves, Optics, Thermodynamics/Notes#Simple Harmonic Motion#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#The Phase Constant|The Phase Constant]]
	- [[Waves, Optics, Thermodynamics/Notes#Energy|Energy]]
	- [[Waves, Optics, Thermodynamics/Notes#Dynamics|Dynamics]]
	- [[Waves, Optics, Thermodynamics/Notes#Vertical Oscillations|Vertical Oscillations]]
	- [[Waves, Optics, Thermodynamics/Notes#Simple Pendulums|Simple Pendulums]]
- [[Waves, Optics, Thermodynamics/Notes#Introduction to Waves|Introducion to Waves (15.1-15.9)]] 
	- [[Waves, Optics, Thermodynamics/Notes#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#Travelling Waves|Travelling Waves]]
	- [[Waves, Optics, Thermodynamics/Notes#Standing Waves|Standing Waves]]
# Simple Harmonic Motion

>[!Textbook]- 
><u>Chapter 14</u>: ![[Giancoli.pdf#page=422|Chapter 14]] 
### variables:
| **name**                   | **symbol** | **unit**                       |
| :------------------------- | :--------- | :----------------------------- |
| $\text{frequency}$         | $f$        | $\text{HZ} \text{ or } s^{-1}$ |
| $\text{period}$            | $T$        | $s$                            |
| $\text{angular frequency}$ | $\omega$   | $\text{HZ}$                    |
| $\text{phase constant}$    | $\phi_0$   |                                |
### equations:
- $f = \dfrac{1}{T}$  
- $\omega = 2\pi f$
- $x(t) = A\cos(\omega t + \phi_0)$
- $v_{max}=\omega A$
- $v_{x}(t) = sin(\omega t + \phi_0)$
- $E = \dfrac{1}{2}mv^{2} + \dfrac{1}{2}kx^2$
- $\omega = \sqrt{\dfrac{k}{m}}$
- $\frac{1}{2}mv^{2} + \frac{1}{2}kx^{2}=\frac{1}{2}kA^{2}$
- $a_{x} = - \omega^{2}x$ 

## Introduction
Oscillatory motion describes repetitive motion about an equilibrium point. Simple Harmonic Motion (SHM) is a type of oscillatory motion where the position and velocity are sinusoidal.

Recall frequency $f$ and period $T$ have an inverse relationship, so:
- $f = \frac{1}{T}$

We can model the motion of a pendulum from rest with the following equation:
- $x(t) = A\cos(\omega t)$, where
- $\omega = 2\pi f = \dfrac{2 \pi}{T}$
## The Phase Constant 
The phase constant $\phi_{0}$ accounts for the offset of SHM, like if the motion does not begin at rest $x = A$, thus augmenting our original equation to:
- $x(t) = A\cos(\omega t + \phi_0)$

Thus, we can calculate the phase constant as:
- $\phi_{0} = \arccos\left(\frac{x(t)}{A}\right) - \omega t$  
## Energy
Energy is conserved in SHM, recall the equations of a spring:
- $E = K + U = \frac{1}{2}mv^{2} + \frac{1}{2}kx^{2}$

Thus at position $x = 0$, kinetic energy is maximized:
- $E(x = 0) = K_{max} = \frac{1}{2}v_{max}^2$ 

And thus at velocity $v = 0$, potentially energy is maximized:
- $E(v=0) = U_{max} = \frac{1}{2}kA^2$ 

By conservation, $K_{max} = U_{max}$ and we derive the following properties:
- $\frac{1}{2}mv^{2} + \frac{1}{2}kx^{2}=\frac{1}{2}kA^{2}$
- $\frac{1}{2}mv_{max}^{2}=\frac{1}{2}kA^2$, which derives:
- $v_{max}=\sqrt{\dfrac{k}{m}}A$, which derives:
- $\omega = \sqrt{\dfrac{k}{m}}$, 
- $f = \dfrac{1}{2\pi}\sqrt{\dfrac{k}{m}}$, 
- $T = 2\pi\sqrt{\dfrac{m}{k}}$ 
## Dynamics
We can derive the acceleration $a_{x}$ of a system in the following manner:
- $a_{x} = \dfrac{dv_{x}}{dt} = \dfrac{d}{dt}(-\omega A \sin(\omega t)) = - \omega A \cos(\omega t)$
- $a_{x} = - \omega^{2}x$ 
- $a_{max} = - \omega^{2}A$
## Vertical Oscillations
Consider a hanging spring, which not only observes the SHM properties, but also has the effects of gravity. We calculate the maximum stretch of the string as:
$\Delta L = \dfrac{mg}{k}$
## Simple Pendulums
A swinging pendulum is one of the most common problems in SHM. It obeys many of the same properties we've referenced for springs, but gains the additional property of angle $\theta$ (measured from the rest position $x = 0$). We also reference the amplitude $A$ as $s$ (for arc-length)
- $-mg\sin(\theta) \approx -mg \\\ \theta = -mg\dfrac{s}{L}$ 
- $s_{max} = \dfrac{v_{max}}{\omega}$ 

# Introduction to Waves
>[!Textbook]- 
><u>Chapter 15</u>: ![[Giancoli.pdf#page=451|Chapter 15]] 

### variables:
| **name**             | **symbol** | **unit**       |
|:-------------------- |:---------- |:-------------- |
| $\text{wavelength}$  | $\lambda$  | $m$            |
| $\text{wave speed}$  | $v$        | $\dfrac{m}{s}$ |
| $\text{wave number}$ | $k$        | $\dfrac{1}{m}$ |
### equations:
- $D(x,t) = A \sin(kx + \omega t)$
- $v = \lambda f$ 
- $v = \sqrt{\dfrac{F_T}{\mu}}$
- $k = \dfrac{2\pi}{\lambda}$
- $D(x,t) = 2A\sin(kx)\cos(\omega t)$
- $\lambda_{m}=\dfrac{2l}{m}$ 
- $f_{m}=\dfrac{mv}{2l} = m \cdot f_{1}$  

## Introduction
We define a wave as a disturbance through a medium, and have an amplitude $A$, a frequency $f$, a wave speed $v$, and a wavelength $\lambda$
We can relate three of these properties as:
- $v = \lambda f$

## Travelling Waves
A travelling wave is a wave whose medium moves in the direction of propagation. We're heavily interested in transverse waves, being waves that oscillate perpendicularly to the direction of movement. For something like a wave through a string with tension $F_T$ and mass per unit length $\mu = \dfrac{m}{l}$ we can calculate the wave speed as:
- $v = \sqrt{\dfrac{F_T}{\mu}}$
We can also derive an equation for a wave travelling to the *right* as:
- $D(x,t) = A \sin(kx - \omega t)$
And its leftward counterpart:
- $D(x,t) = A\sin(kx+\omega t)$
We may also see a *phase constant* version:
- $D(x,t) = A\sin(kx-\omega t + \phi_0)$ 

**The principle of superposition**: The collision two waves $D_1$ and $D_2$ results in a net displacement $D_{3}=D_{1}+D_{2}$ 

When a wave encounters a boundary, like a wall holding the end of a cord in-place, the wave will be reflected, resulting in an inversion of that wave with an equal amplitude. When a wave encounters a change in material, like a cord transitioning to another cord of a different thickness, part of it will be reflected and part of it will be transmitted to the new material. Critically, the frequency does NOT change across mediums, but the velocity $v$ and wavelength $\lambda$ will.

## Standing Waves
Standing waves are waves that do not appear to move, commonly created by moving a cord with fixed ends. The creation of waves and the reflection of those waves by the fixed end ends up creating *nodes*, points of destructive interference with no oscillation, and *anti-nodes*, points of constructive interference with maximum amplitude. 
We can construct the equation of a standing wave as:
- $D(x,t) = 2A\sin(kx)\cos(\omega t)$

The possible standing waves are called the *modes* $m$ of a string, where the value $m$ equals the number of anti-nodes. The mode $m=1$ is known as the fundamental mode. 
Nodes are spaced $\dfrac{\lambda}{2}$ apart, thus the nodes of a standing wave occur at:
- $x_{m}=\dfrac{m\lambda}{2}, m\in\mathbb{N}$ 
On a cord of length $l$, we can calculate the wavelength $\lambda$ as:
- $\lambda_{m}=\dfrac{2l}{m}, m\in\mathbb{N}$ 
And the frequency $f$ as:
- $f_{m}=\dfrac{mv}{2l} = m \cdot f_{1}$  
Subsequently, we can find the frequency of the fundamental mode $f_{1}$ as:
- $f_{1}=\Delta f = f_{m+1} - f_{m}$ 