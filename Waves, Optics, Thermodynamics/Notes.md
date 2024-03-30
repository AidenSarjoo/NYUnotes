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

**The principle of superposition**: The collision two waves $D_1$ and $D_2$ results in a net displacement $D=D_{1}+D_{2}$ 

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

# Sound Waves
>[!Textbook]- 
><u>Chapter 16</u>: ![[Giancoli.pdf#page=484|Chapter 16]] 

### variables:
| **name**             | **symbol** | **unit**       |
|:-------------------- |:---------- |:-------------- |
| $\text{Intensity}$  | $I$  | $\dfrac{W}{m^{2}}$            |
| $\text{sound level}$  | $\beta$        | $dB$ |
### equations:
- $I = \dfrac{P}{a}$
- $\beta = 10 \log(\dfrac{I}{I_{0}})$
- $f_{o} = f_{s} \dfrac{v\pm v_{o}}{v\pm v_{s}}$
- $f_{beat} = |f_{1} - f_{2}|$
### constants:
| **name**             | **symbol** |**value**        | **unit** |
|:-------------------- |:---------- |:-------------- |:-----------|
| $\text{Intensity}$  | $I_0$  | $1.0 \times 10^{-12}$  | $\dfrac{W}{m^{2}}$ |

## Introduction to Sound
Sound waves are *longitudinal waves* (occasionally called *pressure waves*), as opposed to transverse waves, being waves that oscillate in the direction they travel.
An important constant is the speed of sound $v$, which is $331 \frac{m}{s}$ at $1 \text{atm}, 0\degree C$ in air. Note, this changes based on temperature, roughly:
- $v \approx (331 + 0.60 T) \dfrac{m}{s}$, where $T$ is in $\degree C$

Generally, we assume $v = 343 \dfrac{m}{s}$ ($20 \degree C$)

Often, we consider problems with instruments of various shapes, and thus its important to note 3 cases in order to calculate the fundamental frequencies $f_1$:
1. String instruments: $f_{1} = \dfrac{1}{2L}\sqrt{\dfrac{F_{T}}{\mu}}$
2. Open-open tube instruments (flute): $f_{1} = \dfrac{v}{2L}$
3. Open-closed tube instruments (clarinet): $f_{1} = \dfrac{v}{4L}$

Note, $v$ refers to speed of air in the tube 

## Intensity 
Intensity $I$ and power $P$ are important concepts in sound. The power $P$ of a wave is the rate ($J/s$) at which the wave transfers energy. We define intensity $P$ as the power-to-area $a$ ratio:
- $I = \dfrac{P}{a}$

Note, the human ear does not process intensity linearly, and it instead follows a logarithmic curve. For this reason, we consider sound level $\beta$, calculated as:
- $\beta = 10 \log(\dfrac{I}{I_{0}})$

## Doppler Shift
The doppler shift explains the relationship between a frequency at the source $f_o$ and at the observer $f_s$ when either of those entities are moving. We often refer to the following chart:

| Doppler Shift $f_{o} = f_{s} \dfrac{v\pm v_{o}}{v\pm v_{s}}$ | Stationary observer |Observer moving towards source| Observer moving away from source |
|:-------------------- |:---------- |:-------------- |:-----------|
| Stationary source  | $f_{o} = f_{s}   | $f_{o} = f_{s} \dfrac{v + v_{o}}{v}$  | $f_{o} = f_{s} \dfrac{v - v_{o}}{v}$ |
| Source moving towards observer  | $f_{o} = f_{s} \dfrac{v}{v - v_{s}}$  | $f_{o} = f_{s} \dfrac{v + v_{o}}{v - v_{s}}$  | $f_{o} = f_{s} \dfrac{v - v_{o}}{v - v_{s}}$ |
| Source moving away from observer  | $f_{o} = f_{s} \dfrac{v}{v + v_{s}}$  | $f_{o} = f_{s} \dfrac{v + v_{o}}{v + v_{s}}$  | $f_{o} = f_{s} \dfrac{v - v_{o}}{v + v_{s}}$ |

Note that memorizing this chart is not necessary. Observe the base form:
- $f_{o} = f_{s} \dfrac{v\pm v_{o}}{v\pm v_{s}}$
Consider the following cases:
- If the observer is stationary: the numerator is $v$
- If the observer is moving towards the source: the numerator is $v + v_o$, the observed frequency will be higher 
- If the observer is moving away from the source: the numerator is $v - v_o$, the observed frequency will be lower
- If the source is stationary: the denominator is $v$
- If the source is moving towards the observer: the denominator is $v - v_s$, the observed frequency will be higher
- If the source is moving away from the observer, the denominator is $v + v_s$, the observed frequency will be lower

## Interference and Beats
Recall from the principle of superposition that two waves operating on the same space will result in a collision, known as interference. Sound waves, naturally, do the same. Consider the special cases of the waves $D_{1} = a\sin(kx_{1} - \omega t + \phi_{1}), D_{2} = a\sin(kx_{2}-\omega t + \phi_{2})$:
1. $D_{1}(x) = D_2(x)$: the two waves are *in-phase*, meaning their resulting amplitude $A$ is $A = 2a$
2. $D_{1}(x) = -D_2(x)$: the two waves are *out of phase*, meaning their resulting amplitude $A$ is $A = 0$
In the first case, the amplitude is doubled, and in the second case, there is no sound at all.

If two waves of equal amplitude $A$ and frequency $f$ are traveling together, we can write:
- $D = D_{1} + D_{2} = a\sin(\phi_{1})+a\sin(\phi_{2})$
Otherwise, we can write:
- $D = \left[2a\cos\left(\dfrac{\Delta\phi}{2}\right)\right]\sin(kx_{avg}-\omega t + \phi_{avg})$

Observe the following two cases of $\Delta\phi$:
1. $\Delta \phi = m \cdot2\pi$ or $\cos\left(\dfrac{\Delta\phi}{2}\right) = \pm1$: the amplitude $A$ is maximized as $A = 2a$
2. $\Delta\phi = (m + \frac{1}{2})\cdot2\pi$ or $\cos\left(\frac{\Delta\phi}{2}\right)=0$: the amplitude $A$ is minimized as $A = 0$

We now introduce the concept of a *beat*, which is the result of the superposition of sounds from two sources with equal amplitude $a$, but different frequencies $f$.  We can calculate the frequency of the beat $f_{beat}$ as:
- $f_{beat} = 2f_{mod} = 2 \dfrac{\omega_{mod}}{2\pi} = 2 \cdot \frac{1}{2}\left(\dfrac{\omega_{1}}{2\pi} - \dfrac{\omega_{2}}{2\pi}\right) = |f_{1} - f_{2}|$
