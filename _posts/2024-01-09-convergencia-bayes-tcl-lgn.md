---
tags: statistics
title: Convergência, Teorema de Bayes, TCL e LGN
#published: false
sidebar:
    nav: docs-en
---

## Convergência

Definição: Dizemos que uma sequência de variáveis aleatórias $Z_n$ converge para b, se para todo $\epsilon>0$, temos que:

$$\lim \text{Pr}\left(\left|Z_n-b\right|<\epsilon\right)=1$$

## Teorema de Bayes e Probabilidade Condicional
Probabilidade Condicional de B dado A:

$$\begin{gathered}
\text{Pr}(B \mid A)=\text{Pr}(A \cap B) \text{Pr}(B) \\
\text{Pr}(B \mid A)=\frac{\text{Pr}(A \mid B) \text{Pr}(B)}{\text{Pr}(A \mid B) \text{Pr}(B)+\text{Pr}(A \mid \bar{B}) \text{Pr}(\bar{B})}
\end{gathered}$$

## Teorema Central do Limite (TCL)

Para qualquer distribuição de X, com média $\mu$ e variância $\sigma^2$, então para $n \rightarrow \infty$ :

$$\left(\bar{X}_n-\mu\right) / \sigma_{\bar{X}} \rightarrow N(0,1)$$

$N(0,1)$ : Normal padronizada ou Distribuição Normal Padrão.

$$\bar{X}_n \sim N\left(\mu, \sigma^2 / n\right)$$

Ps:. $X$ pode ser qualquer variável aleatória, seja ela discreta ou contínua.

## Lei dos Grandes Números (LGN)

Sejam ( $\left.X_1, X_2, \ldots, X_n\right)$ variáveis aleatórias independentes e identicamente distribuidas com média $\mu$, então:

$$\begin{gathered}
\bar{X}_n=\frac{1}{n} \sum x_i \rightarrow \mu \\
\text{Pr}\left(\lim _{n \rightarrow \infty} \bar{X}_n=\mu\right)=1
\end{gathered}$$
