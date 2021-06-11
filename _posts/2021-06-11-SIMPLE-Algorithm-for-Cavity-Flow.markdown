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


$$u \frac{\partial u}{\partial x}+v \frac{\partial u}{\partial y}=-\frac{1}{\rho} \frac{\partial p}{\partial x}+\nu\left(\frac{\partial^{2} u}{\partial x^{2}}+\frac{\partial^{2} u}{\partial y^{2}}\right)$$

$$u \frac{\partial v}{\partial x}+v \frac{\partial v}{\partial y}=-\frac{1}{\rho} \frac{\partial p}{\partial y}+\nu\left(\frac{\partial^{2} v}{\partial x^{2}}+\frac{\partial^{2} v}{\partial y^{2}}\right)$$
## Discretization Method


## code


## Results
