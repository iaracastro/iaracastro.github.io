---
tags: statistics
title: Região Crítica e de Rejeição
#published: false
sidebar:
    nav: docs-en
---

## Região Crítica

Se queremos rejeitar $H_0$ (hipótese nula) se $\bar{X}_n$ está longe de $\mu_0$. Para isso definimos

$$S_0:= \{x:-c \leq \bar{X}_n-\mu_0 \leq c \}$$

de modo que $S_1=S_0^C$. Então, seguimos o procedimento:

$$\begin{aligned}
& X \in S_1 \Longrightarrow \text { rejeitar } H_0, \\
& X \in S_0 \Longrightarrow \text { não rejeitar } H_0
\end{aligned}$$

Seja $T:= | \bar{X}_n-\mu_0 |$, rejeitamos $H_0$ se $T \geq c$.

---

O conjunto

$$S_1:= \{x: | \bar{X}_n-\mu_0 | \geq c \}$$

é cham ado de região crítica do teste.

## Região de Rejeição

Se $R \subseteq \mathbb{R}$ é tal que dizemos que "rejeitamos $H_0$ se $T \in R$ ", então $R$ é chamada uma região de rejeição para a estatística $T$ e o teste associado.

### Relação de Região Crítica e de Rejeição

Podemos relacionar os conceitos de região crítica e região de rejeição notando queremos

$$S_1:=\{x: r(x) \in R\}$$

### Construindo um teste de tamanho $\alpha_0$
Se $T=r(X)$ é uma estatística, podemos quase sempre encontrar c tal que valha

$$\sup _{\theta \in \Omega_0} \operatorname{Pr}(T \geq c \mid \theta) \leq \alpha_0$$

ou seja, encontrar c tal que $\delta$ tenha tamanho (ou nível de significância) $\alpha_0$.
