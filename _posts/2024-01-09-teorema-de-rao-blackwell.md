---
tags: statistics
title: Teorema de Rao-Blackwell
#published: false
sidebar:
    nav: docs-en
---

## Definição 

O teorema Rao-Blackwell diz que todo estimador condicionado em uma estatística suficiente é admissível.
Seja $\delta(X)$ um estimador, T uma estatistica suficiente para $\theta$ e seja $\delta_0(T)$ um estimador condicionado, então:

$$R\left(\theta, \delta_0\right) \leq R(\theta, \delta)$$

### Melhoramento de Blackwell ou Rao-Blackwellização

O teorema de Rao-Blackwell (às vezes chamado de teorema de Rao-Blackwell-Kolmogorov ou Rao-Blackwellization) é uma maneira de melhorar a eficiência dos estimadores iniciais. Estimadores são variáveis aleatórias observáveis usadas para estimar quantidades. Por exemplo, a média amostral (observável) é um estimador para a média populacional (desconhecida).
O melhoramento de Blackwell condiciona a estatística suficiente.
