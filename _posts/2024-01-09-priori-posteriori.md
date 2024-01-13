---
tags: statistics
title: Priori e Posteriori
#published: false
sidebar:
    nav: docs-en
---


## Priori e Posteriori: $\xi(\theta) & \xi(\theta \mid x)$

Em probabilidade bayesiana, uma distribuição de probabilidade a priori para uma quantidade indeterminada p, também chamada simplesmente de prior relativo a p (suponha, por exemplo, que p seja a proporção de votantes em determinado político numa eleição futura) é a distribuição de probabilidade que expressaria a incerteza sobre o valor de p antes de qualquer dado ou medida (por exemplo, uma pesquisa de opinião). É uma maneira de atribuir incerteza em vez de aleatoriedade à grandeza em questão, além de ponto de partida para o uso do teorema de Bayes após a obtenção dos dados. Já a probabilidade a posteriori de um evento aleatório ou uma proposição incerta é a probabilidade condicionada que é atribuída depois que evidências ou planos de fundo relevantes são levados em conta. De forma semelhante, a distribuição de probabilidade a posteriori é a distribuição de probabilidade de uma quantidade incerta, tratada como uma variável aleatória, condicional sobre a evidência obtida de um experimento ou survey.

$$\xi(\theta \mid x)=\frac{\xi(\theta) \prod_{i-1}^n f_n\left(x_i \mid \theta\right)}{g_n(x)}$$

### Função de Verossimilhança: $f\left(x_1, x_2, \ldots, x_n \mid \theta\right)$

Em estatística, a função de verossimilhança ou função de probabilidade é uma função dos parâmetros de um modelo estatístico que permite inferir sobre o seu valor a partir de um conjunto de observações.

$$\xi(\theta \mid x) \propto f(x \mid \theta) \xi(\theta)$$
