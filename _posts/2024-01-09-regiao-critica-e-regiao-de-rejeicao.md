---
tags: statistics
title: Região Crítica e de Rejeição
#published: false
sidebar:
    nav: docs-en
---

## Região Crítica

Se queremos rejeitar $H_0$ (hipótese nula) se $\bar{X}_n$ está longe de $\mu_0$. Para isso definimos

$$S_0:=\left\{x:-c \leq \bar{X}_n-\mu_0 \leq c\right\}$$

de modo que $S_1=S_0^C$. Então, seguimos o procedimento:

$$\begin{aligned}
& X \in S_1 \Longrightarrow \text { rejeitar } H_0, \\
& X \in S_0 \Longrightarrow \text { não rejeitar } H_0
\end{aligned}$$

Seja $T:=\left|\bar{X}_n-\mu_0\right|$, rejeitamos $H_0$ se $T \geq c$.

---

O conjunto

$$S_1:=\left\{x:\left|\bar{X}_n-\mu_0\right| \geq c\right\}$$

é chamado de região crítica do teste.

## Região de Rejeição

Se $R \subseteq \mathbb{R}$ é tal que dizemos que "rejeitamos $H_0$ se $T \in R$ ", então $R$ é chamada uma região de rejeição para a estatística $T$ e o teste associado.

### Relação de Região Crítica e de Rejeição

Podemos relacionar os conceitos de região crítica e região de rejeição notando queremos

$$S_1:=\{x: r(x) \in R\}$$
