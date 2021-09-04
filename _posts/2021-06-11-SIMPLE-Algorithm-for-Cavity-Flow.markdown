---
layout: single
title:  "Simple Algrithm for Cavity Flow"
date:   2021-06-11 09:08:55 +0800
#categories: iOS
mathjax: true

excerpt: "Basic principles and Python code for cavity flow with SIMPLE algorithm at steady staye"
header:
  teaser: /assets/images/codeback.jpg
  overlay_image: /assets/images/codeback.jpg
  overlay_filter: 0.4 # same as adding an opacity of 0.5 to a black background

---

{% include toc title="Contents" %}

## Governing Equations
Imcompressible flow in the cavity at steady state is elliptical. The two-dimensional governing equation for the cavity flow is,

Mass conservation:

$$\frac{\partial u}{\partial x} + \frac{\partial u}{\partial y} = 0$$

Momentum conservation:

$$u \frac{\partial u}{\partial x}+v \frac{\partial u}{\partial y}=-\frac{1}{\rho} \frac{\partial p}{\partial x}+\nu\left(\frac{\partial^{2} u}{\partial x^{2}}+\frac{\partial^{2} u}{\partial y^{2}}\right)$$

$$u \frac{\partial v}{\partial x}+v \frac{\partial v}{\partial y}=-\frac{1}{\rho} \frac{\partial p}{\partial y}+\nu\left(\frac{\partial^{2} v}{\partial x^{2}}+\frac{\partial^{2} v}{\partial y^{2}}\right)$$

## Discretization Method
SIMPLE(Semi-Implicit Method for Pressure Linked Equations) method is designed to solve the incompressible flow, where the pressure acts as the dependent variable. The implicit discretization for the $\textbf{u}$ momentum equation is,

$$
\begin{aligned}
&\frac{u_{i, j}^{n+1}-u_{i, j}^{n}}{\Delta t}+u_{i, j}^{n} \frac{u_{i+1/2, j}^{n+1}-u_{i-1/2, j}^{n+1}}{\Delta x}+v_{i, j}^{n} \frac{u_{i, j+1/2}^{n+1}-u_{i, j-1/2}^{n+1}}{\Delta y}= \\
&-\frac{1}{\rho} \frac{p_{i+1, j}^{n+1}-p_{i, j}^{n+1}}{\Delta x} \\
&+\nu\left(\frac{u_{i+3/2, j}^{n+1}-2 u_{i+1/2, j}^{n}+u_{i-1/2, j}^{n+1}}{\Delta x^{2}}+\frac{u_{i, j+3/2}^{n+1}-2 u_{i, j}^{n}+u_{i, j-1/2}^{n+1}}{\Delta y^{2}}\right)
\end{aligned}
$$

Similarly for the $\textbf{v}$ momemtum equation is

$$
\begin{gathered}
\frac{v_{i, j}^{n+1}-v_{i, j}^{n}}{\Delta t}+u_{i, j}^{n} \frac{v_{i, j+1/2}^{n+1}-v_{i, j-1/2}^{n+1}}{\Delta x}+v_{i, j}^{n} \frac{v_{i, j+1/2}^{n+1}-v_{i, j-1/2}^{n+1}}{\Delta y}= \\
-\frac{1}{\rho} \frac{p_{i, j+1}^{n+1}-p_{i, j}^{n+1}}{\Delta y} \\
+\nu\left(\frac{v_{i+3/2, j}^{n+1}-2 v_{i+1/2, j}^{n}+v_{i-1/2, j}^{n+1}}{\Delta x^{2}}+\frac{v_{i, j+3/2}^{n+1}-2 v_{i, j}^{nArrheniusArrheniusArrheniusArrhenius}+v_{i, j-1/2}^{n+1}}{\Delta y^{2}}\right)
\end{gathered}
$$

Where the fraction index is from staggered mesh as

$$<>_{i+a/2, j+b/2} = \frac{<>_{i+a/2+1, j+b/2+1}+<>_{i+a/2-1, j+b/2-1}}{2}$$

where $a, b\in \{-3, -2, -1, 0, 1, 2, 3 \}$.

Well

Chutianwei



## Code


## Results
