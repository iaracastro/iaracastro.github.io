![image](https://github.com/iaracastro/iaracastro.github.io/assets/84725802/8892d32f-d080-46b4-8826-7dd3293ae28d)---
tags: real-analysis
title: Números Naturais
#published: false
sidebar:
    nav: docs-en
---

## Axiomas de Peano

$\mathrm{O}$ conjunto $\mathbb{N}$ dos números naturais é caracterizado pelos seguintes fatos:

1. Existe uma função injetiva $s: \mathbb{N} \rightarrow \mathbb{N}$. A imagem $s(n)$ de cada número natural $n \in \mathbb{N}$ chama-se o sucessor de $n$. Ou seja, todo número natural tem um sucessor, que ainda é um número natural. \
2. Existe um único número natural $1 \in \mathbb{N}$ tal que $1 \neq s(n)$ para todo $n \in \mathbb{N}$. Ou seja, existe um único número natural 1 que não é sucessor de nenhum outro. \
3. Se um conjunto $X \subset \mathbb{N}$ é tal que $1 \in X$ e $s(X) \subset X$ (isto é, $n \in X \Rightarrow s(n) \in X)$ então $X=\mathbb{N}$. Ou seja, se um conjunto de números naturais contém o número 1 e cada um dos seus sucessores, então esse conjunto contém todos os números naturais.

Essas afirmações são conhecidas como **Axiomas de Peano**, e 3. é conhecido como o **Princípio da Indução**.

## Princípio da Indução

Seja X um conjunto tal que:

i) $1 \in X$ \
ii) Para todo $n \in \mathbb{N}$, temos que $n \in X \rightarrow n + 1 \in X$ \
Então $X = \mathbb{N}$

### Princípio da Indução Matemática

Seja $P$ uma proposição acerca dos números naturais. Suponhamos que $P$ seja tal que:

1. $P[1]$ vale, isto é, 1 verifica a proposição $P$; \
2. Se $P[k]$ vale, então vale $P[k+1]$, isto é, se $k$ verifica a proposição $P$, então seu sucessor $k+1$ também a verifica.

Então, $P$ é válida para todos os números naturais.

## Operações Fundamentais

- associatividade: $(m+n)+p=m+(n+p), m \cdot(n \cdot p)=(m \cdot n) \cdot p$;
- distributividade: $m \cdot(n+p)=m \cdot n+m \cdot p$;
- comutatividade: $\quad m+n=n+m, m \cdot n=n \cdot m$;
- monotonicidade: Se $m < n \text{ então } mp < np$;
- lei do corte: $\quad m+n=m+p \Rightarrow n=p, m \cdot n=m \cdot p \Rightarrow n=p$.

## Conjuntos Finitos

Continuaremos usando a notação $I_n=\{p \in \mathbb{N} ; p \leq n\}$.
Um conjunto $X$ diz-se finito quando é vazio ou então existem $n \in \mathbb{N}$ e uma bijeção $f: I_n \rightarrow X$. Escrevendo $x_1=f(1), x_2=f(2), \ldots$, $x_n=f(n)$ temos então $X=\left\{x_1, x_2, \ldots, x_n\right\}$. A bijeção $f$ chama-se uma contagem dos elementos de $X$ e o número $n$ chama-se o número de elementos, ou número cardinal do conjunto finito $X$.

- Todo subconjunto de um conjunto finito é finito.
- Um subconjunto $X \subset \mathbb{N}$ é finito se, e somente se, é limitado.

## Conjuntos Infinitos

Diz-se que um conjunto é infinito quando não é finito. Assim, $X$ é infinito quando não é vazio nem existe, seja qual for $n \in \mathbb{N}$, uma bijeção $f: I_n \rightarrow X$.

- Se X é um conjunto infinito, então existe uma aplicação injetiva $f: \mathbb{N} \rightarrow X$.
- Um conjunto $X$ é infinito se, e somente se, existe uma bijeção $\varphi: X \rightarrow Y$ sobre um subconjunto próprio $Y \subset X$.

## Conjuntos Enumeráveis

Um conjunto $X$ diz-se enumerável quando é finito ou quando existe uma bijeção $f: \mathbb{N} \rightarrow X$. Neste caso, $f$ chama-se uma enumeração dos elementos de $X$. Escrevendo $f(1)=x_1, f(2)=x_2, \ldots, f(n)=x_n, \ldots$ tem-se então $X=\left\{x_1, x_2, \ldots, x_n, \ldots\right\}$.

- Todo subconjunto $X \subset \mathbb{N}$ é enumerável.
- Seja $f: X \rightarrow Y$ injetiva. Se $Y$ é enumerável então $X$ também é. Em particular, todo subconjunto de um conjunto enumerável é enumerável.
- O produto cartesiano de dois conjuntos enumeráveis é um conjunto enumerável.
- A reunião de uma família enumerável de conjuntos enumeráveis é enumerável.

### Exemplos

1. O conjunto $\mathbb{Z}=\{\ldots,-2,-1,0,1,2, \ldots\}$ dos números inteiros é enumerável. Uma bijeção $f: \mathbb{N} \rightarrow \mathbb{Z}$ pode ser definida pondo $f(n)=(n-1) / 2$ para $n$ ímpar e $f(n)=-n / 2$ para $n$ par. \
2. O conjunto $\mathbb{Q}=\{m / n ; m, n \in \mathbb{Z}, n \neq 0\}$ dos números racionais é enumerável. Com efeito, escrevendo $\mathbb{Z}^* = \mathbb{Z} - \{0\}$, podemos definir uma função sobrejetiva $f: \mathbb{Z} \times \mathbb{Z}^* \rightarrow \mathbb{Q}$ pondo $f(m, n)=m / n$.
