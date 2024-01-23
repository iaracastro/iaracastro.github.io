---
tags: real-analysis
title: Intervalos e Topologia
#published: false
sidebar:
    nav: docs-en
---

## Definição de Intervalos

### Intervalos Limitados, Ilimitados, Abertos e Fechados

Seja $\mathbb{K}$ um corpo ordenado e $a, b \in \mathbb{K}$ tais que $a < b$. Definimos os intervalos:

1. Intervalo Fechado: $[a, b]:=\{x \in \mathbb{K}: a \leq x \leq b\}$ \
Tal intervalo representa o conjunto de todos os elementos de $\mathbb{K}$ que estão entre $a$ e $b$, inclusive os extremos $a$ e $b$.

2. Intervalo Aberto: $(a, b):=\{x \in \mathbb{K}: a < x < b\}$ \
Neste caso, tal intervalo representa o conjunto de todos os elementos de $\mathbb{K}$ que estão entre $a$ e $b$, menos os extremos $a$ e $b$. Geometricamente, representamos o intervalo $(a, b)$ por
Repare que os extremos $a$ e $b$ são representados por bolas "furadas". Esta simbologia serve para indicar que $a$ e $b$ não pertencem ao intervalo, são apenas limitantes do mesmo.

4. Intervalo Misto: $[a, b):=\{x \in \mathbb{K}: a \leq x < b\}$ 
5. Intervalo Misto: $(a, b]:=\{x \in \mathbb{K}: a < x \leq b\}$ 
6. Intervalo Limitado à esquerda: $(-\infty, b]:=\{x \in \mathbb{K}: x \leq b\}$

#### Exemplos

$$\begin{array}{ll}
{[a, b]=\{x \in \mathbb{R} ; a \leq x \leq b\}} & (-\infty, b]=\{x \in \mathbb{R} ; x \leq b\} \\
(a, b)=\{x \in \mathbb{R} ; a<x<b\} & (-\infty, b)=\{x \in \mathbb{R} ; x<b\} \\
{[a, b)=\{x \in \mathbb{R} ; a \leq x<b\}} & {[a,+\infty)=\{x \in \mathbb{R} ; a \leq x\}} \\
(a, b]=\{x \in \mathbb{R} ; a<x \leq b\} & (a,+\infty)=\{x \in \mathbb{R} ; a<x\} \\
& (-\infty,+\infty)=\mathbb{R}
\end{array}$$

Os quatro intervalos da esquerda são limitados, com extremos $a, b$ : $[a, b]$ é um intervalo fechado, $(a, b)$ é aberto, $[a, b)$ é fechado à esquerda e $(a, b]$ é fechado à direita. Os cinco intervalos à direita são ilimitados.

#### Intervalos encaixantes 
Definição Se $I_n = [a_n, b_n]$ é uma sequêcia de intervalos tal que $I_{n+1} \subseteq I_n \forall n \in \mathbb{N}$, então, $\cap_{n=1}^{\infty} I_n \neq ø$, ou seja, existe pelo menos um número real $c$ tal que $c \in I_n$ para todo $n \in \mathbb{N}$.

## Definição de Conjuntos

### Pontos Interiores
Diz-se que o ponto $a$ é interior ao conjunto $X \subset \mathbb{R}$ quando existe um número $\varepsilon>0$ tal que o intervalo aberto $(a-\varepsilon, a+\varepsilon)$ está contido em $X$. 

### Conjuntos Abertos

O conjunto dos pontos interiores a $X$ chama-se o interior do conjunto $X$ e representa-se pela notação int $X$. Quando $a \in \text{ int } X$ diz-se que o conjunto $X$ é uma vizinhança do ponto $a$. Um conjunto $A \subset \mathbb{R}$ chamase aberto quando $A= \text{ int } A$, isto é, quando todos os pontos de $A$ são interiores a $A$.

a) Se $A_1$ e $A_2$ são conjuntos abertos então a interseção $A_1 \cap A_2$ é um conjunto aberto. \
b) Se $(A_\lambda)$, onde $\lambda \in L$, é uma familia qualquer de conjuntos abertos, a reunião $A=\cap_{\lambda \in L} A_\lambda$ é um conjunto aberto.

### Pontos Aderentes

Diz-se que um ponto $a$ é aderente ao conjunto $X \subset \mathbb{R}$ quando $a$ é limite de alguma seqüência de pontos $x_n \in X$. Evidentemente, todo ponto $a \in X$ é aderente a $X$ : basta tomar $x_n=a$ para todo $n \in \mathbb{N}$.

- Um ponto a é aderente ao conjunto X se, e somente se, toda vizinhança de a contém algum ponto de X.

### Fecho
Chama-se fecho de um conjunto $X$ ao conjunto $\bar{X}$ formado por todos os pontos aderentes a $X$. Tem-se $X \subset \bar{X}$. Se $X \subset Y$ então $\bar{X} \subset \bar{Y}$. 

- O fecho de qualquer conjunto é um conjunto fechado. (Ou seja, $X = \bar{X}$ para todo $X \subset \mathbb{R}$.)
  
### Conjuntos Fechados

Um conjunto $X$ diz-se fechado quando $X=\bar{X}$, isto é, quando todo ponto aderente a $X$ pertence a $X$. Seja $X \subset Y$. Diz-se que $X$ é denso em $Y$ quando $Y \subset \bar{X}$, isto é, quando todo $b \in Y$ é aderente a $X$. Por exemplo, $\mathbb{Q}$ é denso em $\mathbb{R}$.

- Um conjunto $F \subset R$ é fechado se, e somente se, seu complementar $A = \mathbb{R} — F$ é aberto.

a) Se $F_1$ e $F_2$ são fechados então $F_1 \cup F_2$ é fechado. \
b) Se $\left( F_\lambda \right)_{\lambda \in L}$ é uma família qualquer de conjuntos fechados então a interseção $F = \cap_{\lambda \in L} $F_\lambda$ é um conjunto fechado.

### Pontos de Acumulação

Diz-se que $a \in \mathbb{R}$ é ponto de acumulação do conjunto $X \subset \mathbb{R}$ quando toda vizinhança $V$ de $a$ contém algum ponto de $X$ diferente do próprio a. (Isto é, $V \cap(X-\{a\}) \neq \varnothing$.) Equivalentemente: para todo $\varepsilon>0$ tem-se $(a-\varepsilon, a+\varepsilon) \cap(X-\{a\}) \neq \varnothing$. Indica-se com $X'$ o conjunto de pontos de acumulação de $X$.

Dados $X \subset \mathbb{R}$ e $a \in \mathbb{R}$, as seguintes afirmações são equivalentes: \
(1) a é um ponto de acumulação de $X$; \
(2) a é limite de uma seqüência de pontos $x_n \in X-\{a\}$; \
(3) Todo intervalo aberto de centro a contém uma infinidade de pontos de $X$

### Conjuntos compactos

Um conjunto $X \subset \mathbb{R}$ chama-se compacto quando é limitado e fechado.

- Um conjunto $X \subset \mathbb{R}$ é compacto se, e somente se, toda sequência de pontos em $X$ possui uma subsequência que converge para um ponto de $X$.
