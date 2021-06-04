---
layout: single
title:  "Laplace transformation solutions for one heat conduction equation"
date:   2021-06-04 09:08:55 +0800
#categories: iOS
mathjax: true

excerpt: "Laplace transformation solutions for one heat conduction equation"
header:
  teaser: /assets/images/codeback.jpg
  overlay_image: /assets/images/codeback.jpg
  overlay_filter: 0.4 # same as adding an opacity of 0.5 to a black background

---

{% include toc title="Contents" %}

## Laplace transformation solutions for one heat conduction equation

A typical heat conduction equation needs to be solved when taking convection is that a panel with length $L$ is heated. One side at $x=0$ has the convective boundary condition as $\dot{q}^{\prime \prime} = h(T_g-T_s)$, where $h$ is the convective heat transfer coefficient, $T_g$ is the ambient temperature outside and $T_s$ is the temperature at $x=0$. Another boudanry condition is adabatic as $\dot{q}^{\prime \prime} = 0$. The initial condition is that the panel is at $T_{\infty}$.

The governing equation is

$$
\frac{\partial^{2} T}{\partial x^{2}}-\frac{1}{\kappa} \frac{\partial T}{\partial t}=0, \quad a<x<b
$$

where $\kappa$ is the inverse of the thermal diffusivity $\alpha$ for mathmatical further simplications.

Mutiple by $e^{-p t}$ and integrate with respect to $t$ from 0 to $\infty$, which gives the Laplace transformation as,

  $$
\int_{0}^{\infty} e^{-p t} \frac{\partial^{2} T}{\partial x^{2}} d t-\frac{1}{\kappa} \int_{0}^{\infty} e^{-p t} \frac{\partial T}{\partial t} d t=0
$$

For Laplace transformation,

$$
L\left\{\frac{\partial v}{\partial t}\right\}=p L\{v\}-v_{0}
$$

$$
L\left\{\frac{\partial^{n} v}{\partial x^{n}}\right\}=\frac{\partial^{n} \tilde{v}}{\partial x^{n}}
$$

That turns the governing equation as,

$$
\frac{d^{2} [T]}{d x^{2}}-\frac{p}{\kappa} [T]=-\frac{1}{\kappa} T_{0}(x)
$$

where $[T]$ is the Laplace transformed variable.

In this way, the partial differential equation is reduced to the ordinary differential equation.

Write for shortness that $q^2 = \frac{p}{\kappa}$, the equation will become,

$$
\frac{d^{2} [T]}{d x^{2}}-q^2 [T]=-\frac{1}{\kappa} T_{0}(x)
$$

Two solutions exist for the ordinary equation as $B^{q x}$ and $A e^{-q x}$. Bacasue the temperature is bounded as $x \rightarrow \infty$, $A e^{-q x}$ is taken.

The boundary condition at $x = 0$ for the subsidiary equation, the equation after Laplace transformation, is,

 $$
\frac{d [T]}{d x}-h [T]=\frac{h T_g}{p}
$$

The solution satisfies the boundary condition is,

$$
[T]=\frac{h T_{g} e^{-q x}}{p(q+h)}
$$

The inverse Laplace transformation for it is,

$$
v=V \operatorname{erfc} \frac{x}{2 \sqrt{(\kappa t)}}-V e^{h x+h^{2} \kappa l} \operatorname{erfc}\left(\frac{x}{2 \sqrt{(} \kappa t)}+h \sqrt{\kappa t}\right)
$$
