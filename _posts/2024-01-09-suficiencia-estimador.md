---
tags: statistics
title: Suficiência de um estimador
#published: false
sidebar:
    nav: docs-en
---

## Suficiência

Dizemos que uma estatística $T(\theta)$ é suficiente para calcular a verossimilhança. Então também é suficiente para calcular qualquer inferência que dependa apenas dos dados da função de verossimilhança, como EMV e qualquer coisa baseada em distribuição a posteriori. Em outras palavras, a distribuição condicional da amostra dado o valor da estatística não depende de $\theta$.

$$f\left(X_1, X_2, \ldots, X_n \mid T=t, \theta\right)=f\left(X_1, X_2, \ldots, X_n \mid T=t, \theta^{\prime}\right), \forall \theta, \theta^{\prime} \in \Omega$$

Para cada t, a distribuição condicional de $X_1, X_2, \ldots, X_n$ dado $\mathrm{T}=\mathrm{t}$ e $\theta$ é a mesma para todos os $\theta$. Então T é uma estatística suficiente para $\theta$.

### Suficiência Conjunta
Quando a estatística suficiente não é representada por um único valor, e sim um vetor de valores. $T=t_1, \ldots$ e $T_k=t_k$ não depende de $\theta$.

- Vale o teorema da fatorização.
- Exemplos: Normal e Uniforme.

### Suficiência Mínima

Definição 1: Uma estatística T é dita mínima suficiente se T é suficiente e é função de qualquer outra estatística suficiente. Analogamente, um vetor $T= \{ T_1, T_2, \ldots, T_k \}$ é dito minimamente suficiente conjunto se é função de qualquer outro vetor de estatísticas suficientes. \
Definição 2: Uma estatística T é mínima suficiente se para cada estatística T' e para todo $x, y \in X$, $T(x)=T(y)$ sempre que $T^{\prime}(x)=T^{\prime}(y)$. Em outras palavras, T é uma função de $\mathrm{T}^{\prime}$.

### Teorema

Os estimadores de Bayes e de máxima verossimilhança (EMV) são estatísticas minimamente suficientes.

Prova:

- EMV: Se T é uma estatística suficiente para $\theta$ e existe uma EMV única de $\theta$, então a EMV deve ser uma função de $T$.

$$f_x(x \mid \theta) \propto v[r(x), \theta]$$

- Bayes: Escrever a perda esperada a posteriori explicitamente usando a verossimilhança na forma do TF.
