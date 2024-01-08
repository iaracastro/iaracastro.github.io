---
tags: probability
title: V.A Discretas
#published: false
sidebar:
    nav: docs-en
---

#### Função de Probabilidade
Seja $X$ uma variável aleatória discreta, definimos a funçăo de probabilide de $X$ :
$$p_X(x)=Pr(X-x)$$

#### Função de Probabilidade Conjunta
$$p_{X, Y}(x, y)-Pr(X-x \mathrm{e} Y-y)$$

#### Distribuição Marginal
Oferece as probabilidades de vários valores das variáveis no subconjunto sem referenciar aos valores das outras variáveis.
Seja $p(x, y)=P(X=x, Y=y)$ a funçào de probabilidade conjunta de $\mathrm{X}$ e $\mathrm{Y}$.
$$f(x)=P(X-x)=\sum_n p(x, y)$$

Exemplo:
$$\begin{array}{cccc}
Y & 1 & 2 & 3 \\
0 & 0.4 & 0.1 & 0.1 \\
1 & 0 & 0.2 & 0.2
\end{array}$$

Fazendo o total dentro de cada colune cucontranes a distribuicão marginal de $X$ :
$$\begin{array}{cccc}
x & 1 & 2 & 3 \\
Pr(X=x) & 0.4 & 0.3 & 0.3
\end{array}$$

####  Distribuição Condicional
Valor de $X$ é conhecido, então a distribuição de $Y$ é condicional dado aquele valor de $X=x$. Exemplo: valor de $Y$. No exemplo ackia, a distribuçóo condicional de $X$ dodo que $Y=0$ é simplesmente
$$Pr(X-x \mid Y=0) \quad \frac{1}{6} \quad \frac{1}{6} \quad \frac{1}{6}$$

Variáveis Aleatórias Discretas Indepententes
$$\begin{gathered}
Pr(X=i, Y=j)=Pr(X=i) \cdot Pr(Y=j) \\
Pr(X=i Y=j)=\frac{Pr(X=i \text { e } Y=j)}{Pr(Y=j)}=Pr(X=i)
\end{gathered}$$

Função de Probabilidade Acumulada
$$F_X(x)=Pr(X<x)$$
