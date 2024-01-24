---
tags: real-analysis
title: Sequências de Números Reais
#published: false
sidebar:
    nav: docs-en
---

Uma seqüência de números reais é uma função $x: \mathbb{N} \rightarrow \mathbb{R}$, que associa a cada número natural $n$ um número real $x_n$, chamado o $n$-ésimo termo da seqüência.

Escreve-se $\left(x_1, x_2, \ldots, x_n, \ldots\right)$ ou $\left(x_n\right)_{n \in \mathbb{N}}$, ou simplesmente $\left(x_n\right)$, para indicar a seqüência cujo $n$-ésimo termo é $x_n$.

### Sequência Limitada

- Uma sequência $\left(x_n\right)$ diz-se **limitada superiormente** quando existe $c \in \mathbb{R}$ tal que $x_n \leq c$ para todo $n \in \mathbb{N}$. 
- Analogamente, uma sequência se diz **limitada inferiormente** quando existe $c \in \mathbb{R}$ tal que $x_n \leq c$ tal que $x_n \geq c$ para todo $n \in \mathbb{N}$. 

Diz-se que a sequência $\left(x_n\right)$ é limitada quando ela é limitada superior e inferiormente. Isto equivale a dizer que existe $k > 0$ tal que $|x_n| \leq k$ para todo $n \in \mathbb{N}$. 

### Limite de Sequência

Dada uma sequência de números reais $\left(a_1, a_2, a_3, \ldots\right)$, dizemos que $L=\lim a_n$ se para qualquer $\epsilon>0$ existe um inteiro positivo $N(\epsilon)$ tal que para todo $n \geq N(\epsilon)$ temos que:

$$\left|a_n-L\right|<\epsilon$$

### Operações com Limites

- Se $\lim x_n=0$ e $\left(y_n\right)$ é uma seqüência limitada (convergente ou não) então $\lim \left(x_n \cdot y_n\right)=0$.
- Se $\lim x_n=a$ e $\lim y_n=b$ então:
1. $\lim \left(x_n \pm y_n\right)=a \pm b$.
2. $\lim \left(x_n \cdot y_n\right)=a \cdot b$.
3. $\lim \frac{x_n}{y_n}=\frac{a}{b}$ se $b \neq 0$.

### Limites Infinitos

Dada uma seqüência $\left(x_n\right)$, $\lim x_n=+\infty$, se dado arbitrariamente $A>0$, existe $n_0 \in \mathbb{N}$ tal que $n > n_0$ implica $x_n>A$.

Analogamente, dada uma seqüência $\left(x_n\right)$, $\lim x_n= -\infty$, se dado arbitrariamente $A < 0$, existe $n_0 \in \mathbb{N}$ tal que $n > n_0$ implica $x_n < A$.

#### Propriedades

(1) Se $\lim x_n=+\infty$ e $\left(y_n\right)$ é limitada inferiormente então $\lim \left(x_n+\right.$ $\left.y_n\right)=+\infty$ \
(2) Se $\lim x_n=+\infty$ e existe $c>0$ tal que $y_n>c$ para todo $n \in \mathbb{N}$ então $\lim \left(x_n y_n\right)=+\infty$ \
(3) Se $x_n>c>0, y_n>0$ para todo $n \in \mathbb{N}$ e $\lim y_n=0$ então $\lim \frac{x_n}{y_n}=+\infty$ \
(4) $S e\left(x_n\right)$ é limitada e $\lim y_n=+\infty$ então $\lim \frac{x_n}{y_n}=0$.

### Subsequências

Uma subsequência de uma sequência é uma função $s: \mathbb{N}^{\prime} \rightarrow \mathbb{R}$, onde $\mathbb{N}^{\prime} \subset \mathbb{N}$ e $\mathbb{N}^{\prime}$ é infinito. A notação usual para representar uma subsequência é $\left(a_n\right)_{n \in \mathbb{N}^{\prime}}$.

Como $\mathbb{N}^{\prime}$ é enumerável, seus elementos podem ser escritos como $\left\{n_1, n_2, \ldots, n_k, \ldots\right\}$, e ainda podemos escolher a enumeração de forma com que $n_i<n_j$, se $i<j$. Então podemos identificar uma subsequência com uma sequência escrevendo $\left(a_{n_k}\right)_{k \in \mathbb{N}}$. Portanto, todos os teoremas que valem para sequências valem para subsequências.
### Subsequência

Uma subsequência de uma sequência $\left(a_n\right)$, com $n \in \mathbb{N}$, é uma função $s: \mathbb{N}^{\prime} \rightarrow \mathbb{R}$, onde $\mathbb{N}^{\prime} \subset \mathbb{N}$ e $\mathbb{N}^{\prime}$ é infinito. A notação usual para representar uma subsequência é $\left(a_n\right)_{n \in \mathbb{N}^{\prime}}$.

Como $\mathbb{N}^{\prime}$ é enumerável, seus elementos podem ser escritos como $\{n_1, n_2, \ldots, n_k, \ldots\}$, e ainda podemos escolher a enumeração de forma com que $n_i<n_j$, se $i<j$. Então podemos identificar uma subsequência com uma sequência escrevendo $\left(a_{n_k}\right)$, com $k \in \mathbb{N}$. Portanto, todos os teoremas que valem para sequências valem para subsequências.

### Teoremas de Sequências

- Unicidade do Limite: Uma sequência não pode convergir para dois limites distintos.
- Se $\lim x_n=a$ então toda subseqüência de $\left(x_n\right)$ converge para o limite a.
- Toda seqüência convergente é limitada.
- Toda seqüência monótona limitada é convergente.

### Teorema de Bolzano-Weierstrass 

Toda sequência limitada de números reais possui uma subseqüência convergente.

### Valores de Aderência
Os valores de aderência de uma sequência são os limites de suas subsequências convergentes (podem não existir, mas se a sequência é convergente somente há um valor de aderência). 

- Bolzano-Weierstrass: Se a sequência é limitada, sempre existem valores de aderência.
  
### Teorema do sanduíche

Se $\lim x_n = \lim y_n=a$ e $x_n \leq z_n \leq y_n$ para todo $n$ suficientemente grande então $\lim z_n=a$.
