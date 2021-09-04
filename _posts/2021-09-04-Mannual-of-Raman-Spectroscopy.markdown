---
layout: single
title:  "Manual of Raman Spectroscopy"
date:   2021-09-04 09:08:55 +0800
#categories: iOS
mathjax: true

excerpt: "Mannual of the self-made Raman Sprectroscopy in FireLab of HKPolyU"
header:
  teaser: /assets/images/Raman_cover.png
  overlay_image: /assets/images/Raman_cover.png
  overlay_filter: 0.4 # same as adding an opacity of 0.5 to a black background

---

{% include toc title="Contents" %}

# Introduction

Raman spectroscopy (RS) is a non-destructive spectroscopic technique used to determine the vibration modes of molecules, although rotational and other low-frequency models may be observed. Raman spectroscopy is commonly used to find a structural fingerprint of molecules in chemistry. 
Since the characteristics that RS can identify different vibrational frequencies which are specific to chemical bonds, such technique is widely used in biology, medicine, combustion and so on. In solid state physics, RS is used to measure the temperature and crystallographic orientation of a sample. In solid-state chemistry, RS can be used to identify active pharmaceutical ingredients and their polymorphic forms. RS helps to confirm the low-frequency of DNA and proteins in biology and medicine. Explosives, pollutant and other desirable species can be detected with portable RS devices in practice which is also widely in use. In the field of combustion, RS is also one of the approaches for combustion diagnostics. Lapp and Hartley gives a comprehensive review of such technique in combustion. RS can identify species in combustion field and measure the species fraction or temperature as well. With the high-frequency pulsed laser source, RS can realize one-dimensional measurements for combustion field. Another advanced technique is Coherent Anti-Stokes Raman Spectroscopy(CARS), which can extensively eliminate the effect of fluorescence and surrounding noise, albeit with higher cost. 
RS developed in the laboratory is a primitive facility for point measurement of species and designed to measure the species fractions and temperature in the future. 

# Instrument Components

RS consists of two major components, the sample chamber and the spectroscopy together with two affiliated components, optical fiber transmitter and standard light source. The descriptions of different components in the spectroscopy are listed. 

{% include figure image_path="/assets/images/Spectroscopy.png" alt="Sprectroscopy" caption="Compotents in the spectroscopy" %}

## 2.1 Sample chamber

# Instrument Principles
## Background

Three conditions exist when the light hits the materials. If the material is homogeneous and there is no heat fluctuations, no interactions appear between the lights and the materials. The lights got through from the materials dos not change and the wavelength and the direction do not change consequently. If the material is non-homogeneous and non-dynamics heat fluctuations exist, the direction of the light through the materials changes and the frequency does not change. Such phenomena is recognized as the elastic scattering. If dynamic heat fluctuation of the material exists, energy exchanges between the lights and the materials appear, the frequency changes, which is known as the inelastic scattering. The inelastic scattering was firstly proposed by Smekal in 1923 and observed by C.V. Raman in 1923 from the 423.85nm lights through the tetrachloromethane solution. The inelastic scattering is named as Raman scattering since then. The technique was not put into practice at the beginning because the intensity of Raman scattering is about 10-6 of the incident light, which makes the scattering difficult to be observed and quantified. The Raman Spectroscopy technique boosts around 1970s because of the emerging of laser. The performance as monochrome, intensity, directivity and polarization is excellent of laser. Laser thus becomes the popular excitation source form Raman spectroscopy. Anther boost is the development of Charge Coupled Device (CCD), which can massively reduce the measing period. Meanwhile, other techniques flourish such as Surface-enhanced Raman Spectroscopy (SERS), Resonance Raman Spectroscopy (RRS), Coherent Anti-Stokes Raman Scattering (CARS) and so on. In the field of combustion, CARS is the popular diagnostic method to measure the species, fractions and temperature of the gas phase.

## Theories

$$
\begin{aligned}
&\boldsymbol{A}=\boldsymbol{A}_{0}+\sum_{k=1}^{3 N-6}\left(\frac{\partial \boldsymbol{A}}{\partial q_{k}}\right)_{0} Q_{k} \cos \left(\omega_{k} t+\varphi_{k}\right) \\
&+\frac{1}{2} \sum\left(\frac{\partial^{2} \boldsymbol{A}}{\partial q_{k} \partial q_{1}}\right) Q_{k} Q_{l} \cos \left(\omega_{k} t+\varphi_{k}\right) \cos \left(\omega_{l} t+\varphi_{l}\right)+\cdots
\end{aligned}
$$