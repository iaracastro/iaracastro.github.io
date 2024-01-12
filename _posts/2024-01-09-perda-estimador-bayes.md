---
tags: probability
title: Funções de Perda e Estimadores de Bayes
#published: false
sidebar:
    nav: docs-en
---

## Funções de Perda: $L(\theta, \delta)$

Uma função de perda especifica uma penalidade para uma estimativa incorreta de um modelo estatístico. Funções de perda típicas podem especificar a penalidade em função da diferença entre a estimativa e o valor real.

### Perda Quadrática:

$$L(\theta, \delta)-(\delta-\theta)^2$$

### Perda Absoluta:

$$L(\theta, \delta)=|\delta-\theta|$$

## Estimador de Bayes: $\theta_{\text {bayes }}=E[\theta \mid \bar{x}]$

### Definição

Estimador que minimiza a funçăo de perca a posteriori.

$$E[L(\theta, \delta(\bar{x})) \mid \bar{x}]=\int_{\Omega} L(\theta, \delta) \xi(\theta, x)$$

- Na perda quadrátca: $\theta_{\text {buye }}=$ média da posteriori
- Na perda absoluta: $\theta_{\text {suyes }}=$ mediana da posteriori

### Exemplos:

$\text{Gamma}(\alpha, \rho):$

$$\delta=\frac{\alpha+n \bar{x}}{\beta+n}=\frac{\alpha+y}{\beta+n}, y=\sum_1^n x_i$$

$\text{Bet} \alpha(\alpha, \beta):$

$$\delta^*=\frac{\alpha}{\alpha+\beta}$$

- Se $x_1, \ldots, x_n$ é uma distribuiçäo de poisson $x_i \mid \theta \propto P(\theta)$ e a priori for uma distribuiçäo Gamma $\theta \sim G(\alpha, \beta)$ então a posteriori também é uma distribuição Gamma.
- Se $x_1, \ldots, x_n$ é uma distribuição uniforme $x_i \mid \theta \sim U(0, \theta)$ e a priori for uma distribuição de Pareto $\theta \sim P a\left(\theta_0, a\right)$ entāo a posteriori também é uma distribuiçāo de Pareto.
