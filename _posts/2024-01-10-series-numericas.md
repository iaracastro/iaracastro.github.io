---
tags: real-analysis
title: Séries Numéricas
#published: false
sidebar:
    nav: docs-en
---

Uma série é uma soma $s=a_1+a_2+\cdots+a_n+\cdots$ com um número infinito de parcelas. Para que isto faça sentido, poremos $s=\lim _{n \rightarrow \infty}\left(a_1+\right.$ $\left.\cdots+a_n\right)$. Como todo limite, este pode existir ou não. Por isso há séries convergentes e séries divergentes. 

Dada uma seqüência $\left(a_n\right)$ de números reais, a partir dela formamos uma nova seqüência $\left(s_n\right)$ onde

$$s_1=a_1, \quad s_2=a_1+a_2, \quad \ldots, \quad s_n=a_1+a_2+\cdots+a_n, \text { etc. }$$

Os números $s_n$ chamam-se as reduzidas ou somas parciais da série $\sum a_n$. A parcela $a_n$ é o $n$-ésimo termo ou termo geral da série.

## Séries Convergentes e Divergentes

Se existir o limite $s= \lim_{n \rightarrow \infty} s_n$, diremos que a série $\sum a_n$ é convergente e $s=\sum a_n=\sum_{n=1}^{\infty} a_n=a_1+a_2+\cdots+a_n+\cdots$ será chamado a soma da série. Se $\lim s_n$ não existir, diremos que $\sum a_n$ é uma série divergente.

### Exemplos

-  a série geométrica: $1+a+a^2+\cdots+a^n+\cdots$, onde $|$ $a$ $|$<1$, é convergente, com soma igual a $1 /(1-a)$.
-  a série $1+1+1 / 2 !+\cdots+1 / n !+\cdots$ também converge, com soma igual a $e$.
-  a série $1-1+1-1+\cdots$, de termo geral $(-1)^{n+1}$, é divergente pois a soma parcial $s_n$ é igual a zero quando $n$ é par, e igual a 1 quando $n$ é ímpar. Portanto não existe $\lim s_n$.
-  a série $\sum 1 / n(n+1)$, cujo termo geral é $a_n=1 / n(n+1)=$ $1 / n-1 /(n+1)$, tem $n$-ésima soma parcial

$$s_n=\left(1-\frac{1}{2}\right)+\left(\frac{1}{2}-\frac{1}{3}\right)+\cdots+\left(\frac{1}{n}-\frac{1}{n+1}\right)=1-\frac{1}{n+1}$$

- a **série harmônica** $\sum \frac{1}{n}$ é divergente.

## Série Absolutamente Convergente

Uma série $\sum a_n$ diz-se absolutamente convergente quando $\sum$ $\left|$ $a_n$ $\right|$ converge.

### Exemplo

Uma série convergente cujos termos não mudam de sinal é absolutamente convergente. Quando $-1 < a < 1$, a série geométrica $\sum_{n=0}^{\infty} a^n$ é absolutamente convergente, pois $\left|$ $a^n$ $\right|$ $=|a|^n$, com $0 \leq$ $|$ $a$ $|$ $< 1$.

## Testes de Convergência

### Critério de Comparação

**Definição:** Sejam $\sum a_n e \sum b_n$ séries de termos não-negativos. Se existem $c>0$ e $n_0 \in \mathbb{N}$ tais que $a_n \leq c b_n$ para todo $n>n_0$ então a convergência de $\sum b_n$ implica a de $\sum a_n$ enquanto a divergência de $\sum a_n$ implica a de $\sum b_n$.

Seja $\sum b_n$ uma série absolutamente convergente, com $b_n \neq$ 0 para todo $n \in \mathbb{N}$. Se a seqüência $\left(a_n / b_n\right)$ for limitada (em particular, se for convergente) então a série $\sum a_n$ será absolutamente convergente.
Demonstração: Se, para algum $c>0$, tivermos $\left|a_n / b_n\right| \leq c$. seja qual for $n \in \mathbb{N}$ então $\left|a_n\right| \leq c\left|b_n\right|$. Pelo critério de comparação, a série $\sum a_n$ é absolutamente convergente.

### Teste de d'Alembert.

Seja $a_n \neq 0$ para todo $n \in$ $\mathbb{N}$. Se existir uma constante $c$ tal que $\left|a_{n+1} / a_n\right| \leq c<1$ para todo $n$ suficientemente grande (em particular, se $\lim \left|a_{n+1} / a_n\right|<1$ ) então a série $\sum a_n$ será abolutamente convergente.

- Usualmente se procura calcular $\lim \left|a_{n+1} / a_n\right|=L$. Se $L>1$ então a série diverge pois se tem $\left|a_{n+1} / a_n\right|>1$, donde $\left|a_{n+1}\right|>\left|a_n\right|$ para todo $n$ suficientemente grande e daí resulta que o termo geral $a_n$ não tende para zero. Se $L=1$, o teste é inconclusivo. A série pode convergir (como no caso $\sum 1 / n^2$ ) ou divergir (como no caso $\sum 1 / n$ ).
  
### Teste de Cauchy

Quando existe um número real c tal que $\sqrt[n]{\left|a_n\right|} \leq c<1$ para todo $n \in \mathbb{N}$ suficientemente grande (em particular, quando $\left.\lim \sqrt[n]{\left|a_n\right|}<1\right)$, a série $\sum a_n$ é absolutamente convergente.

#### Exemplo

Seja $a_n=(\log n / n)^n$. Como $\sqrt[n]{a_n}=\log n / n$ tende a zero, a série $\sum a_n$ é convergente.

## Teoremas

- O termo geral de uma série convergente tem limite zero.
- **Leibniz**: Se ( $a_n$ ) é uma seqüência monótona decrescente que tende para zero então $\sum(-1)^{n+1} a_n$ é uma série convergente.
- Toda série absolutamente convergente é convergente.
- relacão entre os testes de d'Alembert e Cauchy: seja $\left(a_n\right)$ uma seqüência cujos termos são diferentes de zero. Se $\lim \left|a_{n+1}\right| /\left|a_n\right|=L$ então $\lim \sqrt[n]{\left|a_n\right|}=L$.

