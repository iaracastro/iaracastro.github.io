---
tags: probability
title: V.A Contínuas
#published: false
sidebar:
    nav: docs-en
aside:
  toc: true
key: 2024-01-08_en
---

## Distribuição Uniforme

Distribuição de uma variável aleatória $X$ que tem distribuiçăo uniforme no intervalo $[a, b]$

$$\begin{gathered}
f(x)-\left\{\begin{array}{r}
\frac{1}{b-a} ; \text { se } a \leq x \leq b \\
\text { Nâo rejeitar } H_0, \text { se }\left|\bar{X}_b-\mu_0\right|<c
\end{array}\right. \\
F(x)=\left\{\begin{array}{c}
0 \text { se }:<<a \\
\frac{x-a}{b-a}, \text { se } a \leq x \leq b \\
1 \text { se } b<x
\end{array}\right. \\
E[x]=\frac{a+b}{2} \\
Var[x]=\frac{(b-a)^2}{12}
\end{gathered}$$

## Distribuição Exponencial
A distribuição exponencial é a distribuiçāo de probabilidade do tempo entre eventos de um processo de Poisson.

$$\begin{gathered}
f(t)-\left\{\begin{array}{r}
\lambda e^{\lambda t}, \text { se } t>0 \\
0, \text { c.c }
\end{array}\right. \\
F(x)=\left\{\begin{array}{r}
0 \text { se } t<0 \\
1-e^{-\lambda t} \text { se } t>0
\end{array}\right.
\end{gathered}$$

$$X \sim Exp(\lambda)$$

$$\begin{gathered}
E(X)=\frac{1}{\lambda} \\
Var(X)=\frac{1}{\lambda^2}
\end{gathered}$$

## Distribuição Gama

$$\begin{gathered}
\Gamma(\alpha)=\int_0^{\infty} x^{\alpha-1} e^* \\
\Gamma(n)=(n-1) ! \\
\Gamma\left(\frac{1}{2}\right)-\sqrt{\pi} \\
\text { GammaDen }(t)=\left\{\begin{array}{rr}
\frac{\lambda^\alpha}{\Gamma(\alpha)} t^{\alpha-1} e^{-\lambda l}, & \text { se } t>0 \\
0, \text { c.c }
\end{array}\right.
\end{gathered}$$

$$X \sim Gamma(\alpha, \lambda)$$
