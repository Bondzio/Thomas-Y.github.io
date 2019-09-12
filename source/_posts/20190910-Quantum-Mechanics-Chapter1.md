---
title: Fall 2019 Quantum Mechanics Chapter1
date: 2019-09-10 09:15:39
categories:
- [Academic, Physic, Quantum Mechanics]
tags:
- Physic
- Quantum Mechanics
- Learning Notes
mathjax: true
---

摘要：黑体辐射；光电效应；康普顿散射；波尔氢原子模型；Stern-Gerlach实验，角动量与自旋；德布罗意物质波。

<!--more-->

本系列文档为完全基于《Quantum Mechnics》[^1]的学习笔记。

# 1 The origins of quantum theory

## 1.1 Black body radiation

Define ***Absorptance*** $\alpha$ - fraction of incident radiation absorbed.

Define $E_{b}$ - energy radiated per unit area per unit time.

Define ***Black body*** which has properties:  
* $\alpha=1$   
* $E_{b}=\sigma T^{4}$ , where $\sigma$ - the Stefan-Boltzmann constant

$$\sigma=5.67 \times 10^{-8} \ \mathrm{J} \ \mathrm{s}^{-1} \ \mathrm{m}^{-2} \ \mathrm{K}^{-4}$$

Define ***Emissive power*** $e_{\lambda} = d E_{b} / d \lambda \approx \Delta E_{b} / \Delta \lambda$ - the energy radiated per unit area for a range of wavelengths of width $\Delta \lambda$ .

### 1.1.1 Kirchhoff's law[^2]

>For a body of any arbitrary material emitting and absorbing thermal electromagnetic radiation at every wavelength in thermodynamic equilibrium, the ratio of the emissive power to the absorption coefficient is equal to a universal function only of radiative wavelength and temperature.

### 1.1.2 Stefan–Boltzmann law[^3][^4]

 The total energy radiated per unit surface area of a black body across all wavelengths per unit time is only related to its temperature:

 $$E_{b}=\sigma T^{4}$$

Prerequisite:  
* the first and second law of thermodynamic
* Maxwell's electromagnetic theory

Assumption:  
* A box is filled with black body radiation, of which one wall is a piston which is moved by the pressure of the radiation.
* According to classical electromagnetism, the pressure *P* is related to the energy density by $p=\frac{u}{3}$. This equation still holds for the radiation pressure.

Define **u** - energy density

Now we use the heat-energy balance equation $d U=T d S-p d V$ to obtain

$$T d S=d(u V)+P d V=u^{\prime}(T) V d T+u d V+\frac{1}{3} u d V=u^{\prime}(T) V d T+\frac{4}{3} u d V \ .$$

Dividing through by *T* and using the fact that *dS* is a complete differential

$$\frac{\partial}{\partial V}\left(\frac{u^{\prime}(T) V}{T}\right)=\frac{\partial}{\partial T}\left(\frac{4 u}{3 T}\right) \ ,$$

which simplifies, after some algebra, to $u^{\prime}(T)=4 u(T) / T$ , that is, $u(T) \propto T^{4}$ .

Define **n** - number density

Then we quote a result from kinetic theory, namely that the flux of particles striking a unit area of a container is

$$\Phi=\frac{1}{4} n\langle v\rangle=\frac{1}{4} n c \ ,$$

which is also the number of particles striking a unit area of a container per unit time. I have replaced *v* with *c* , and using the fact that power emitted is the flux times the energy per particle , we get

$$E_{b}=\frac{1}{4} n c \frac{u}{n}=\left(\frac{1}{4} c A \right) T^{4} \equiv \sigma T^{4} \ .$$


[^1]: Bransden, B. H., & Joachain, C. J. (2000). Quantum Mechanics (2nd ed.). Harlow, England: Pearson/Prentice Hall.  
[^2]: Kirchhoff, G. (1860), Ueber das Verhältniss zwischen dem Emissionsvermögen und dem Absorptionsvermögen der Körper für Wärme und Licht. Ann. Phys., 185: 275-301. doi:10.1002/andp.18601850205. Translated by Guthrie, Kirchhoff, G. (1860). I. On the relation between the radiating and absorbing powers of different bodies for light and heat. The London, Edinburgh, and Dublin Philosophical Magazine and Journal of Science, 20(130), 1–21. doi:10.1080/14786446008642901.  
[^3]: Knizhnik, Kalman. Derivation of the Stefan–Boltzmann Law. Johns Hopkins University – Department of Physics & Astronomy.  
[^4]: Cardy, J. (2010). The ubiquitous ‘c’: from the Stefan–Boltzmann law to quantum information. Journal of Statistical Mechanics: Theory and Experiment, 2010(10), P10004.
