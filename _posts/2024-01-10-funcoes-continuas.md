---
tags: real-analysis
title: Funções Contínuas 
#published: false
sidebar:
    nav: docs-en
---

## Continuidade de f
Definição: $f:I \rightarrow \mathbb{R}$ é contínua com $a \in I$ se para todo $\epsilon > 0, \exists \; \delta > 0$ tal que:


$$|x-a| < \delta \rightarrow |f(x) - f(a)| < \epsilon$$

Ou: 

$$\lim_{x \rightarrow a} f(x) = f(a)$$

## Continuidade em f'
$$\lim_{x\rightarrow c} f'(x) = f'(c)$$

- Uma função é contínua quando $f$ é contínua em todos seus pontos

## Uniformemente Contínua
Uma função $f:X \rightarrow \mathbb{R}$ diz-se uniformemente contínua no conjunto $X$ quando, para todo $\epsilon>0$ dado arbitrariamente, pode-se obter $\delta>0$ tal que $x,y \in X,$ $|y-x|<\delta$ implicam $|f(y) - f(x)| < \epsilon$ 

## Teorema do Valor Intermediário (T.V.I)
Se $f:I \rightarrow \mathbb{R}$ é contínua e $a,b \in I$, $a < b$ tais que $f(a) < f(b)$, então, para todo $d \in (f(a),f(b))$ existe $c \in (a,b)$ tal que $f(c) = d$.

Corolário: seja $f:[a,b] \rightarrow \mathbb{R}$ contínua, com $f(a) < 0$ e $f(b)>0$. Existe então $c \in(a,b)$ tal que $f(c) = 0$

### Teoremas
- Funções deriváveis são contínuas.
- Funções contínuas são integráveis.
- **(Teorema de Weierstrass)** Seja $f: X \rightarrow \mathbb{R}$ contínua no conjunto compacto $X \subset \mathbb{R}$. Existem $x_0, x_1 \in X$ tais que $f\left(x_0\right) \leq f(x) \leq f\left(x_1\right)$ para todo $x \in X$.
