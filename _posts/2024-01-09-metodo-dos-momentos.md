---
tags: statistics
title: Método dos Momentos 
#published: false
sidebar:
    nav: docs-en
---

# Definição

O estimador de momentos é a solução da igualdade dos momentos amostrais com os momentos populacionais. Em outras palavras, temos um estimador que usa os momentos, dependendo da distribuição são usados 1 ou 2 momentos. Caso haja mais parâmetros, os próximos momentos serão informados. 

Suponha que $X_1, X_2, \ldots, X_n$ formam uma amostra aleatória com distribuição conjunta $f_n\left(X_1, X_2, \ldots, X_n \mid \theta\right), \theta \in \Omega \subseteq \mathbb{R}^k$ e que o $k$-ésimo momento existe. Defina $\mu_j(\theta)=E\left[X_1^j \mid \theta\right]$ e suponha que $\mu: \Omega \rightarrow \mathbb{R}^k$ é biúnivoca, de modo que sua inversa é

$$\theta=M\left(\mu_1(\theta), \ldots, \mu_k(\theta)\right)$$

Dados os momentos amostrais $m_j:=\frac{1}{n} \sum_{i=1}^n X_i^j, j=1, \ldots, k$, o estimador de momentos (EMM) de $\theta$ é

$$\hat{\theta}_{E M M}=M\left(m_1, \ldots, m_k\right)$$ 

## Primeiro Momento

- $\mu_1(\theta)=E[x]=\mu=$ média
- $m_1=\frac{1}{n} \sum_{i=1}^n x_i=\overline{x_n}$

## Segundo Momento

- $\mu_2(\theta)=E\left[x^2\right]$
- $m_2=\frac{1}{n} \sum_{i=1}^n x_i^2$

## Outros momentos para n parâmetros

- $\mu_n(\theta)=E\left[x^n\right]$
- $m_n=\frac{1}{n} \sum_{i=1}^n x_i^n$

### Resolver o sistema de $\mathrm{n}$ equações:

- $\mu_1(\theta)=m_1$
- $\mu_2(\theta)=m_2$ \
. \
. \
. 
- $\mu_n(\theta)=m_n$
