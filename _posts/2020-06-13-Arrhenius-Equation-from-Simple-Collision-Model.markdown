---
layout: single
title:  "Arrhenius Equation from Simple Collision Model"
date:   2021-06-13 09:08:55 +0800
#categories: iOS
mathjax: true

excerpt: "Derive Arrhenius equation from simple molecule collisions"
header:
  teaser: /assets/images/codeback.jpg
  overlay_image: /assets/images/codeback.jpg
  overlay_filter: 0.4 # same as adding an opacity of 0.5 to a black background

---

The Boltzmann distribution is stated as,

$$
\mathcal{P}(v) \mathrm{d} v=\left[\int_{0}^{\pi} \int_{0}^{2 \pi} \mathcal{P}(\vec{v}) v^{2} \sin \theta \mathrm{d} \theta \mathrm{d} \phi\right] \mathrm{d} v=4 \pi \mathcal{P}(\vec{v}) v^{2} \mathrm{~d} v
$$

Explicitly,

$$
\mathcal{P}(v) \mathrm{d} v=4 \pi\left(\frac{m}{2 \pi k T}\right)^{3 / 2} e^{-\frac{m v^{2}}{2 k T}} v^{2}
$$

The averaged velocity from the distribution is,

$$
\langle v\rangle=\frac{\int_{0}^{\infty} v \mathcal{P}(v) \mathrm{d} v}{\int_{0}^{\infty} \mathcal{P}(v) \mathrm{d} v}=\left(\frac{8 k T}{\pi m}\right)^{3 / 2}
$$

For the molecule conllision, the mass is the reduced mass for the molecule $A$ and $B$,

$$
\langle v\rangle_{A B}=\left(\frac{8 k T}{\pi \mu_{\mathrm{AB}}}\right)^{3 / 2}
$$

For a molecule $A$ with the diameter $d$, in a unit time, the molecule can only collise another molecules in the area centering $A$, with radius $d$ and length $v$, the collision cross section is,

$$
\sigma=\pi d^{2}
$$

The diameter for the collision is,

$$
\sigma=\pi d_{\mathrm{AB}}^{2}=\pi\left(\frac{d_{\mathrm{A}}+d_{\mathrm{B}}}{2}\right)^{2}
$$

If the density of the gas is $\rho$, the collision frequency is

$$
\gamma=\rho \sigma\langle v\rangle
$$

The mean free path is,

$$
\lambda=\frac{\langle v\rangle}{\gamma}=\frac{1}{\rho \sigma}
$$

As the mass of $A$ and $B$ are different, the mean free path is modified as

$$
\lambda_{\mathrm{A}}=\frac{\left\langle v_{\mathrm{A}}\right\rangle}{\gamma_{\mathrm{AB}}}=\sqrt{\frac{\mu_{\mathrm{AB}}}{m_{\mathrm{A}}}} \frac{1}{\rho \sigma_{\mathrm{AB}}}
$$

The reaction is,

$$
\sum_{i} v_{i} i=0
$$

The reaction rate is defined as,

$$
\nu=\frac{1}{v_{i}} \frac{\mathrm{d}[i]}{\mathrm{d} t}
$$

For a two-molecule reaction sytem $A$ and $B$, from the mass conservation, the reaction rate is,

$$
\nu=k[A]^{x}[B]^{y}
$$

The reaction rate from the molecule collision is,

$$
\begin{aligned}
\nu &=-\frac{\mathrm{d}[A]}{\mathrm{d} t}=-\frac{\mathrm{d}\left[N_{\mathrm{A}} /\left(\mathcal{N}_{\mathrm{A}} V\right)\right]}{\mathrm{d} t} \\
&=-\frac{1}{\mathcal{N}_{\mathrm{A}} V} \frac{\mathrm{d} N_{\mathrm{A}}}{\mathrm{d} t}=\frac{1}{\mathcal{N}_{\mathrm{A}} V} \frac{N_{\text {coll }} \mathcal{P}_{\mathrm{rxn}}}{\mathrm{d} t}
\end{aligned}
$$

$\mathcal{N}_{\mathrm{A}}$ is denoted as the Avogadro's number, $N_{\text {coll }}$ is the number of the molecule partipating the reaction, $\mathcal{P}_{\text {rxn }}$ is the reaction possibility.

The time derivative of the collision number, dividing by the Avogadro's number and the volume, is the concentration changing as

$$\frac{N_{\text {coll }}}{\mathrm{d} t}=N_{\mathrm{A}} \gamma_{\mathrm{AB}}=\left(\rho_{\mathrm{A}} V\right)\left(\rho_{\mathrm{B}} \sigma_{\mathrm{AB}}\left\langle v_{\mathrm{AB}}\right\rangle\right)$$

The possibility of the reaction is stated as,

$\mathcal{P}_{\text {ran }}=p \cdot \mathcal{P}\left(E_{\mathrm{AB}}>E_{a}\right)$

The statement is from the assumption that when the collision kenetic energy between $A$ and $B$ is beyond a threshold, the reaction can happen. While the reaction cannot be guaranteed, a factor $p$ is added. In this way, the reaction rate is,

$$\nu=\frac{1}{\mathcal{N}_{\mathrm{A}}} \rho_{\mathrm{A}} \rho_{\mathrm{B}} \sigma_{\mathrm{AB}}\left\langle v_{\mathrm{AB}}\right\rangle p \mathcal{P}\left(E_{\mathrm{AB}}>E_{\alpha}\right)$$

Assume that the distribution of molecules that the kenetic enegy is beyond the threshold obeys Boltzmann distribution as

$$
\mathcal{P}\left(E_{\mathrm{AB}}>E_{a}\right)=\frac{\int_{E_{\alpha}}^{\infty} e^{-E_{\mathrm{AB}} / k T} \mathrm{~d} E_{\mathrm{AB}}}{\int_{0}^{\infty} e^{-E_{\mathrm{AB}} / k T} \mathrm{~d} E_{\mathrm{AB}}}=e^{-E_{a} / k T}
$$

Consequencely,

$$
\nu=\frac{1}{\mathcal{N}_{\mathrm{A}}} \rho_{\mathrm{A} .} \rho_{\mathrm{B}} \sigma_{\mathrm{AB}}\left\langle v_{\mathrm{AB}}\right\rangle p e^{-E_{a} / k T}
$$

The reaction rate coefficient is the same as the Arrhenius equation,

$$
k=A e^{-E_{a} / k T}
$$

where $A$ is modelled as,

$$
A=\sigma_{\mathrm{AB}} \sqrt{\frac{8 k T}{\pi \mu_{\mathrm{AB}}}} \mathcal{N}_{\mathrm{A}} p
$$
