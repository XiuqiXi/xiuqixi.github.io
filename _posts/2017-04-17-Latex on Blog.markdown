---
layout: single
title:  "Cold Plasma in Moving Flow"
date:   2021-06-03 09:08:55 +0800
#categories: iOS
mathjax: true

excerpt: "dispersion relation for waves traveling"
header:
  teaser: /assets/images/codeback.jpg
  overlay_image: /assets/images/codeback.jpg
  overlay_filter: 0.4 # same as adding an opacity of 0.5 to a black background

---

{% include toc title="Contents" %}

## Cold Plasma in Moving Flow

Consider a cold plasma made up of electrons and ions with mass $M_{i}$ and electrical charge $Z$. The ions have an equilibrium flow speed $
\mathbf{u}_{o i}$ and the electrons flow so that there in no equilibrium plasma current. There is no equilibrium magnetic field

The equilibrium flows are such that there is no net current. We demand that the plasma is quasi-neutral. This provides a unique relationship between the equilibrium electron and ion density.

### The dielectric tensor for the plasma
$$
0=\operatorname{Zen}_{z 0}-e n_{e 0}
$$

$$
n_{z 0}=\frac{n_{e 0}}{Z}
$$

The no current constraints yields the relationship.

$$
0=n_{z 0} Z e \mathbf{u}_{z 0}-n_{e 0} e \mathbf{u}_{c 0}
$$

Using the above relationship for nz0, we see that the electrons and ion fluids flow with the same speed.

$$
\mathbf{u}_{e 0}=\mathbf{u}_{z 0}
$$

The dielectric relationship is obtained from $\epsilon(\omega, \mathbf{k})=\epsilon_{o} \mathbf{I}+(i / \omega) \overrightarrow{\vec{\sigma}}$ where $\overrightarrow{\vec{\sigma}}$ is the conductivity defnied from

$$
\mathrm{J}=\overrightarrow{\vec{\sigma}} \cdot \mathbf{E}
$$

The linearized current is obtained from,

$$
\tilde{\mathbf{J}}=\sum_{s} q_{s}\left(n_{s o} \tilde{\mathbf{u}}_{s}+\tilde{n}_{s} \mathbf{u}_{s o}\right)
$$

where $\mathbf{u}_{s o}$ is a constant constant equilibrium fluid velocity for both the ions and electrons. We assume wave-like solutions $\sim e^{i \mathbf{k} \cdot \mathbf{x}-i \omega t}$. The fluid velocity response is obtained from the linearized momentum equation

$$
m_{s} n_{s o}\left(-i \omega+i \mathbf{k} \cdot \mathbf{u}_{s o}\right) \tilde{\mathbf{u}}_{s}=q_{s} n_{s o} \tilde{\mathbf{E}}+q_{s} n_{s 0} \mathbf{u}_{s o} \times \tilde{\mathbf{B}}
$$

Using from Faraday's Law $(\nabla \times \tilde{\mathbf{E}}=-\partial \tilde{\mathbf{B}} / \partial t)$, $\tilde{\mathbf{B}}=\mathbf{k} \times \tilde{\mathbf{E}} / \omega$, the pertubated flow vlocity it given by

$$
\tilde{\mathbf{u}}_{s}=i \frac{q_{s}}{m_{s}\left(\omega-\mathbf{k} \cdot \mathbf{u}_{s o}\right)}\left[\tilde{\mathbf{E}}+\frac{1}{\omega} \mathbf{u}_{s o} \times(\mathbf{k} \times \tilde{\mathbf{E}})\right]
$$

$$
\tilde{\mathbf{u}}_{s}=i \frac{q_{s}}{m_{s}\left(\omega-\mathbf{k} \cdot \mathbf{u}_{s o}\right)}\left[\tilde{\mathbf{E}}+\frac{\mathbf{k}}{\omega} \mathbf{u}_{s o} \cdot \tilde{\mathbf{E}}-\frac{\mathbf{k} \cdot \mathbf{u}_{s o}}{\omega} \tilde{\mathbf{E}}\right] .
$$

The density response is

$$
\left(-i \omega+i \mathbf{k} \cdot \mathbf{u}_{s o}\right) \tilde{n}_{s}+i n_{s o} \mathbf{k} \cdot \tilde{\mathbf{u}}_{s}=0
$$

which, in combination with the fluid velocity perturbation gives
$$
\tilde{n}_{s}=n_{s o} \frac{\mathbf{k} \cdot \tilde{\mathbf{u}}_{s}}{\omega-\mathbf{k} \cdot \mathbf{u}_{s o}}=i \frac{q_{s} n_{s o}}{m_{s}\left(\omega-\mathbf{k} \cdot \mathbf{u}_{s o}\right)^{2}}\left[\mathbf{k} \cdot \tilde{\mathbf{E}}\left(1-\frac{\mathbf{k} \cdot \mathbf{u}_{s o}}{\omega}\right)+\frac{k^{2}}{\omega} \mathbf{u}_{s o} \cdot \tilde{\mathbf{E}}\right]
$$
