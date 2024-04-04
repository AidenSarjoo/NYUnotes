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
	- [[Waves, Optics, Thermodynamics/Notes#Introduction to Waves#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#Travelling Waves|Travelling Waves]]
	- [[Waves, Optics, Thermodynamics/Notes#Standing Waves|Standing Waves]]
- [[Waves, Optics, Thermodynamics/Notes#Sound Waves|Sound Waves (16.1-16.4,16.6-16.7)]]
	- [[Waves, Optics, Thermodynamics/Notes#Sound Waves#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#Intensity|Intensity]]
	- [[Waves, Optics, Thermodynamics/Notes#Doppler Shift|Doppler Shift]]
	- [[Waves, Optics, Thermodynamics/Notes#Interference and Beats|Interference and Beats]]
- [[Waves, Optics, Thermodynamics/Notes#Electromagnetic Waves|Electromagnetic Waves (31.1-31.9)]]
	- [[Waves, Optics, Thermodynamics/Notes#Electricity and Magnetism|Electricity and Magnetism]]
	- [[Waves, Optics, Thermodynamics/Notes#Electromagnetic Waves#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#Electromagnetic Waves#Energy|Energy]]
	- [[Waves, Optics, Thermodynamics/Notes#Radiation Pressure|Radiation Pressure]]
- [[Waves, Optics, Thermodynamics/Notes#Polarization|Polarization (34.7)]]
	- [[Waves, Optics, Thermodynamics/Notes#Polarization#Introduction|Introduction]]
- [[Waves, Optics, Thermodynamics/Notes#Reflection and Refraction|Reflection and Refraction (32.2-32.9)]]
	- [[Waves, Optics, Thermodynamics/Notes#Reflection and Refraction#Introduction|Introduction]]
	- [[Waves, Optics, Thermodynamics/Notes#Reflection and Refraction#Specular Reflection|Specular Reflection]
	- [[Waves, Optics, Thermodynamics/Notes#Reflection and Refraction#Refraction|Refraction]]
	- [[Waves, Optics, Thermodynamics/Notes#Reflection and Refraction#LensesLenses]]

# Simple Harmonic Motion
>[!Textbook]- 
><u>Chapter 14</u>: ![[Giancoli.pdf#page=422|Chapter 14]] 
### variables:
| **name**                   | **symbol** | **unit**                       |
| :------------------------- | :--------- | :----------------------------- |
| $\text{frequency}$         | $f$        | $\text{HZ} \text{ or } s^{-1}$ |
| $\text{period}$            | $T$        | $s$                            |
| $\text{angular frequency}$ | $\omega$   | $\text{HZ}$                    |
| $\text{phase constant}$    | $\phi_0$   |                           |
### equations:
- $f = \dfrac{1}{T}$  
- $\omega = 2\pi f$
- $x(t) = A\cos(\omega t + \phi_0)$
- $v_{max}=\omega A$
- $v_{x}(t) = -\omega \sin(\omega t + \phi_0)$
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
| $\text{Threshold of hearing}$  | $I_0$  | $1.0 \times 10^{-12}$  | $\dfrac{W}{m^{2}}$ |

## Introduction
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

Note, the human ear does not process intensity linearly, and it instead follows a logarithmic curve. For this reason, we consider sound level $\beta$, defined as:
- $\beta \equiv 10 \log(\dfrac{I}{I_{0}})$

## Doppler Shift
The doppler shift explains the relationship between a frequency at the source $f_o$ and at the observer $f_s$ when either of those entities are moving. We often refer to the following chart:

| Doppler Shift $f_{o} = f_{s} \dfrac{v\pm v_{o}}{v\pm v_{s}}$ | Stationary observer                  | Observer moving towards source               | Observer moving away from source             |
|:------------------------------------------------------------ |:------------------------------------ |:-------------------------------------------- |:-------------------------------------------- |
| Stationary source                                            | $f_{o} = f_{s}$                       | $f_{o} = f_{s} \dfrac{v + v_{o}}{v}$         | $f_{o} = f_{s} \dfrac{v - v_{o}}{v}$         |
| Source moving towards observer                               | $f_{o} = f_{s} \dfrac{v}{v - v_{s}}$ | $f_{o} = f_{s} \dfrac{v + v_{o}}{v - v_{s}}$ | $f_{o} = f_{s} \dfrac{v - v_{o}}{v - v_{s}}$ | 
| Source moving away from observer                             | $f_{o} = f_{s} \dfrac{v}{v + v_{s}}$ | $f_{o} = f_{s} \dfrac{v + v_{o}}{v + v_{s}}$ | $f_{o} = f_{s} \dfrac{v - v_{o}}{v + v_{s}}$ |

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

# Electromagnetic Waves
>[!Textbook]- 
><u>Chapter 31</u>: ![[Giancoli.pdf#page=921|Chapter 31]] 

### variables:
| **name**                 | **symbol** | **unit**                                |
|:------------------------ |:---------- |:--------------------------------------- |
| $\text{Electric Field}$  | $E$        | $\dfrac{N}{C} \text{ or } \dfrac{V}{m}$ |
| $\text{Magnetic Field}$  | $B$        | $T$                                     |
| $\text{Electric Flux}$   | $\Phi_{e}$ | $V \cdot m$                             |
| $\text{Magnetic Flux}$   | $\Phi_{m}$ | $T \cdot m^{2}$                         |
| $\text{Current}$         | $I$        | $A$                                     |
| $\text{Poynting Vector}$ | $\vec{S}$  | $\dfrac{W}{m^{2}}$                      |
| $\text{Energy Density}$  | $u$        | $\dfrac{J}{m^{3}}$                      |
### equations:
- $\Phi_{e}=  \oint \vec{E} \cdot d\vec{A} = \dfrac{Q_{in}}{\epsilon_{0}}$
- $\Phi_{m} = \oint \vec{B} \cdot d \vec{A} = 0$
- $\varepsilon= \oint \vec{E} \cdot d \vec{s} = - \dfrac{d\Phi_{m}}{dt}$
- $\oint \vec{B} \cdot d \vec{s} = \mu_{0}I_{through}+\mu_{0}\epsilon_{0}\dfrac{d\Phi_{e}}{dt}$
- $\vec{F} = q(\vec{E}+\vec{v}\times \vec{B})$
- $\vec{S} \equiv \dfrac{1}{\mu_{0}}\vec{E}\times \vec{B}$
- $I = \dfrac{c \epsilon_{0}}{2}E_{0}^{2}$
- $I = \dfrac{P_{source}}{4\pi r^{2}}$
- $u_{E}=\frac{1}{2}\epsilon_{0}E^{2}$
- $u_{B}=\frac{1}{2} \dfrac{B^{2}}{\mu_{0}}$
- $u = \epsilon_{0}E^{2}$
- $u_{avg}=\frac{1}{2}\epsilon_{0}E^{2}$
- $I = c \cdot u_{avg}$
- $p_{rad}=\dfrac{I}{c}=\dfrac{F}{A}$
### constants:
| **name**                              | **symbol**   | **value**             | **unit**                |
|:------------------------------------- |:------------ |:--------------------- |:----------------------- |
| $\text{Permittivity of Free Space}$   | $\epsilon_0$ | $8.85 \times10^{-12}$ | $\dfrac{C^{2}}{Nm^{2}}$ |
| $\text{Vacuum magnetic permeability}$ | $\mu_{0}$    | $4\pi \times10^{-7}$  | $\dfrac{Tm}{A}$         |
| $\text{Speed of light}$               | $c$          | $3 \times 10^{8}$     | $\dfrac{m}{s}$          |

## Electricity and Magnetism
Large portions of this section are review of electricity and magnetism content, thus, we gloss over some explanations. 
Recall Gauss' Law for the electric field, stating for a closed surface enclosing charge $Q_{in}$, the net electric flux $\Phi_{e}$ is given by:
- $\Phi_{e}=  \oint \vec{E} \cdot d\vec{A} = \dfrac{Q_{in}}{\epsilon_{0}}$

Recall Gauss' Law for the magnetic field, stating that the net magnetic flux $\Phi_{m}$ through a closed surface is $\Phi_{m}=0$:
- $\Phi_{m} = \oint \vec{B} \cdot d \vec{A} = 0$

Recall Faraday's Law, stating that a changing magnetic flux $\Phi_{m}$ through a loop creates an induced electromagnetic field $\varepsilon$:
- $\varepsilon= \oint \vec{E} \cdot d \vec{s} = - \dfrac{d\Phi_{m}}{dt}$

Recall Ampere's Law, relating the current through a surface $I_{through}$ to magnetic field $B$:
- $\oint \vec{B} \cdot d \vec{s} = \mu_{0}I_{through}$

Though, this equation is imprecise, and we introduce a correction in the form of Ampere-Maxwell's Law, which adds a displacement current $I_{disp}=\epsilon_{0} \dfrac{d\Phi_{e}}{dt}$:
- $\oint \vec{B} \cdot d \vec{s} = \mu_{0}(I_{through}+I_{disp})=\mu_{0}I_{through}+\mu_{0}\epsilon_{0}\dfrac{d\Phi_{e}}{dt}$
This equation elaborates that a magnetic field $B$ can be created either by an electric current $I$ or a changing electric field.

We now introduce the Lorentz Force Law, relating how matter operates in these fields:
- $\vec{F} = q(\vec{E}+\vec{v}\times \vec{B})$

Giancoli summarizes the above as:
- **Gauss' Law for electricity**: Charged particles create an electric field
- **Faraday's Law**: An electric field can also be created by a changing magnetic field
- **Gauss' Law for magnetism**: All magnetic poles are dipoles (they are paired)
- **Ampere-Maxwell's Law, first half**: Currents create a magnetic field
- **Ampere-Maxwell's Law, second half**: A magnetic field can also be created by a changing electric field
- **Lorentz Force Law, first half**: An electric force is exerted on a charged particle in an electric field
- **Lorentz Force Law, second half**: A magnetic force is exerted on a charge moving in a magnetic field


## Introduction 
By understanding that a magnetic field is created by a changing electric field, we can derive that if a changing magnetic field produces an electric field, that electric field is also changing. The change in that electric field then creates a changing magnetic field, and this oscillation creates a wave of fields that propagate through space, and we can this an electromagnetic wave.

The waves move in the same direction with the same speed $c$, but note that the electric waves and the magnetic waves will propagate perpendicularly. Facing the direction of the speed of the wave, the magnetic field wave will propagate $90\degree$ clockwise of the electric wave.

Note that these waves are also $in-phase$, meaning that they maximize and minimize at the same times.

Through effort, we derive the speed of electromagnetic waves $c$ as:
- $c = \dfrac{1}{\sqrt{\epsilon_0\mu_{0}}}$
We can relate the field strengths at any point in the wave of the two fields as:
- $E = cB$

We also define the energy flow of an electromagnetic wave, or the instantaneous ate of energy transfer per unit area of the wave, with the Poynting vector $\vec{S}$, defined as:
- $\vec{S} \equiv \dfrac{1}{\mu_{0}}\vec{E}\times \vec{B}$
We calculate the max of the Poynting vector $S_{max}$ as:
- $S_{max}=\frac{E_{0}^{2}}{c \mu_{0}}$
Critically, the average of the Poynting vector $S_{avg}=\frac{1}{2}S_{max}$ is the intensity $I$, deriving the equation:
- $I = \dfrac{c \epsilon_{0}}{2}E_{0}^{2}$
We can also use the original equation for intensity $I = P/A$ to calculate the intensity of an electromagnetic waves at a distance $r$ away from an equally radiating power source $P$ as:
- $I = \dfrac{P_{source}}{4\pi r^{2}}$

## Energy 
We briefly consider the energy and energy density $u$ of electromagnetic waves:
The energy density in the electric field $u_{E}$ is:
- $u_{E}=\frac{1}{2}\epsilon_{0}E^{2}$

The energy density in the magnetic field $u_{B}$ is:
- $u_{B}=\frac{1}{2} \dfrac{B^{2}}{\mu_{0}}$

Applying conservation of energy $u = u_{E} + u_{B}$ and the relation between electric field and magnetic field $E = cB$, we can derive:
- $u = \epsilon_{0}E^{2}$
- $u = \dfrac{B^{2}}{\mu_{0}}$
- $u = \sqrt{\dfrac{\epsilon_0}{\mu_{0}}}EB$
- $u_{avg} = \frac{1}{2}\epsilon_{0}E^{2}$

Finally, we can relate energy density $u$ to intensity $I$, as:
- $I = c \cdot u_{avg}$

## Radiation Pressure
Electromagnetic waves transmit their momentum into objects, which we refer to as radiation pressure $p_{rad}$, calculated as:
- $p_{rad}=\dfrac{F}{A}=\dfrac{P/A}{c}=\dfrac{I}{c}$

Mainly, we use this to relate intensity $I$ to area $A$ and force $F$:
- $\dfrac{I}{c}=\dfrac{F}{A}$

#  Polarization
>[!Textbook]- 
><u>Chapter 34.7</u>: ![[Giancoli.pdf#page=1033|Chapter 34.7]] 
### equations:
- $E = E_0\cos(\theta)$
- $I = I_{0}\cos^{2}(\theta)$
## Introduction
Polarization is a much smaller topic in optics. We define the plane of polarization as the plane defined by the Poynting vector $\vec{S}$ and the electric field vector $\vec{E}$, and we pay special attention to the direction of the plane: whether it is *vertically polarized* or *horizontally polarized*. For the most part, natural light sources are *unpolarized*, meaning their fields oscillate randomly in all possible orientations, but we do find value in then polarizing these fields through a polarizing filter.

On this polarizing filter, we have a transmission axis with an angle $\theta$ to the incident polarization direction. Passing through this filter, the electric field $E_0$ is then reduced, following the equation:
- $E = E_0\cos(\theta)$

Importantly, we then see a reduction in the intensity $I$, calculated as:
- $I = I_{0}\cos^{2}(\theta)$

When unpolarized light passes through a filter, we expect the polarization to be $E[I] = \frac{1}{2}I_{0}$

Something that occurs commonly is chaining polarizers, such that light passes through multiple polarizing filters, we can calculate the result of these as:
- $I_{n}=I_{0}\prod\limits_{i=0}^{n}\cos^{2}(\theta_{i})$ 

where $\theta_i$ is the angle of the $i^{th}$ polarizing filter relative to the light

# Reflection and Refraction
>[!Textbook]- 
><u>Chapter 32</u>: ![[Giancoli.pdf#page=949|Chapter 32]] 

### variables:
| **name**                     | **symbol** | **unit**     |
|:---------------------------- |:---------- |:------------ |
| $\text{Angle of Incidence}$  | $\theta_i$ | $\text{rad}$ |
| $\text{Angle of Reflection}$ | $\theta_r$ | $\text{rad}$ |
| $\text{Index of Refraction}$ | $n$        |              |
| $\text{Critical Angle of Incidence}$ | $\theta_c$   | $\text{rad}$             |
| $\text{focal length}$ | $f$ | $m$ |
| $\text{radius of curvature}$ | $r$ | $m$ |
| $\text{magnification}$ | $m$ | |
### equations:
- $n = \dfrac{c}{v}$
- $n_{1}\sin(\theta_1)=n_{2}\sin(\theta_2)$
- $\theta_{c} = \arcsin\left(\dfrac{n_{2}}{n_{1}}\right)$ 
- $\lambda' = \dfrac{\lambda}{n}$ 
- $f = \dfrac{r}{2}$
-  $\dfrac{1}{d_{o}} + \dfrac{1}{d_{i}} = \dfrac{1}{f}$
-  $m = \dfrac{h_i}{h_{o}} = \dfrac{d_{i}}{d_{o}}$

## Introduction
This chapter primarily deals with the  light rays, straight-line paths of light, as they bounce and scatter across surfaces. 

## Specular Reflection
When light strikes a perfectly smooth, flat surface and is bounced off, we call this a specular reflection. When a beam of light bounces off this surface, we define the angle between the normal of the surface and the light ray to be the angle of incidence $\theta_i$. Importantly, the angle between the reflected light ray and the normal of the surface is called the angle of reflection $\theta_r$, and it is equal to the angle of incidence $\theta_{i}=\theta_{r}$

In comparison to specular reflection, we have diffuse reflection, in which light strikes a rough surface and is scattered. We will not be addressing diffuse reflection critically.

Specular reflections create what we call a $virtual image$, i.e. the object being reflected in the mirror. For a specular reflection, the distance from the object to the mirror $d_o$ is equal to the distance from the mirror to the virtual object $d_i$.

## Refraction
Refraction refers to the bending of light rays as they traverse between mediums, i.e. from air to water or glass to air. All mediums have what's known as the *index of refraction* $n$, which is understood as the relation between the speed of light $c$ and the speed of light through that medium $v$, calculated as:
- $n = \dfrac{c}{v}$


Importantly, when light traverses through a medium it bends. Consider the angle the incident ray in medium 1 with index of refraction $n_1$ makes with the normal of the surface of medium 2  $\theta_1$ , and the angle the bent ray, or *refracted ray*, makes with the normal of the surface of the medium $\theta_2$. We can relate these two with the following:
- $n_{1}\sin(\theta_1)=n_{2}\sin(\theta_2)$

Based on the relationship between $n_1$ and $n_2$ we can observe the following two cases when a light ray in a medium of $n_1$ crosses a boundary into a medium of $n_2$:
1. If $n_1 > n_2,$ the light ray will bend *away* from the normal of the boundary 
2. If $n_{1} < n_{2},$ the light ray will bend *towards* the normal of the boundary

We now consider the concept of *total internal reflection*, a logical extension of the above concepts. Consider a situation of case 1. As the angle of the incident ray to the normal $\theta_{1}$ increases, the refraction angle $\theta_{2}$ will approach $90 \degree$, until no light is refracted and instead it is entirely reflected into the original medium. We can calculate the value when this occurs, the critical angle of incidence $\theta_{c}$, as:
- $\theta_{c} = \arcsin\left(\dfrac{n_{2}}{n_{1}}\right)$ 

We also observe a change in the wavelength $\lambda$, calculable as:
- $\lambda' = \dfrac{\lambda}{n}$ 
Note that there is no change in frequency $f$ across mediums

We can now consider the creation of virtual images by refraction across mediums. Consider an object in a medium $n_2$ and an observer in medium $n_1$, where the object has some distance from the boundary $d_o$. We create the following relation with the image distance $d_{i}$
- $n_{1}d_{o} = -n_{2}d_{i}$

## Lenses
Lenses are one of the most important concepts in optics. We consider lenses of two main shapes:
1. Converging lenses, or concave lenses, which cause rays to refract towards the optical axis (inwards)
2. Diverging lenses, or convex lenses, which cause rays to refract away from the optical axis (outwards)

These lenses have a property focal length $f$, defined slightly differently for each. For converging lenses, the focal length $f$ is the distance from the lens where parallel rays appear to converge. For diverging lenses, the focal length $f$ is the distance from the lens at which rays parallel to the optical axis appear to diverge. 

We can calculate the focal length $f$ using another measurement, the radius of curvature $r$, as:
- $f = \dfrac{r}{2}$

We can now relate the object distance $d_o$ and the image distance $d_i$ through the focal length $f$ of the lens that creates the virtual image with the following equation:
- $\dfrac{1}{d_{o}} + \dfrac{1}{d_{i}} = \dfrac{1}{f}$

We can also calculate the magnification $m$ of a lens. We define the magnification $m$ to be the ratio of the image height $h_i$ to the object height $h_o$, which is equal to the ratio of the image distance $d_i$ to the object distance $d_{o}$, thus:
- $m = \dfrac{h_i}{h_{o}} = \dfrac{d_{i}}{d_{o}}$
