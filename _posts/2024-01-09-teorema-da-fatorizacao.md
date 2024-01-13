---
tags: statistics
title: Teorema da Fatorização
#published: false
sidebar:
    nav: docs-en
---

### Definição

Se T é suficiente para $\theta$ podemos escrever a verossimilhança como o produto entre uma função que não depende de $\theta$ e uma função que só depende de $\mathrm{X}$ através de $\mathrm{T}$.

$$f_n(x \mid \theta)=u(x) \cdot v(T(x, \theta))$$

Em outras palavras:

- u depende apenas de $x$ (e não de $\theta$ ).
- $\mathrm{v}$ depende de $\theta$ e $\mathrm{x}$, mas depende de $\mathrm{x}$ apenas através de $\mathrm{T}$.
