---
tags: probability
title: V.A Discretas
#published: false
sidebar:
    nav: docs-en
---

### Função de Probabilidade
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

###  Distribuição Condicional
Valor de $X$ é conhecido, então a distribuição de $Y$ é condicional dado aquele valor de $X=x$. Exemplo: valor de $Y$. No exemplo ackia, a distribuçóo condicional de $X$ dodo que $Y=0$ é simplesmente:

$$Pr(X-x \mid Y=0) \quad \frac{1}{6} \quad \frac{1}{6} \quad \frac{1}{6}$$

### Variáveis Aleatórias Discretas Indepententes:

$$\begin{gathered}
Pr(X=i, Y=j)=Pr(X=i) \cdot Pr(Y=j) \\
Pr(X=i Y=j)=\frac{Pr(X=i \text { e } Y=j)}{Pr(Y=j)}=Pr(X=i)
\end{gathered}$$

### Função de Probabilidade Acumulada
$$F_X(x)=Pr(X<x)$$

### Valor Esperado $E(X)$
Também conhecido como esperança matemática, é uma média ponderada dos valores de $X$ com pesos iguais às respectivas probabilidades destes valores.
$$E(X)-\sum_{y \subset S} x \cdot p(x)$$

Propriedades:
$\cdot$ Seja $Y=f(X)$,

$$\begin{gathered}
E(Y)=E(f(X))=\sum_{x \in S} f(x) \cdot p(x) \\
E(a X+b)=a E(X)+b \\
E(b)-0
\end{gathered}$$

$\cdot$  Seja $Z-f(X, Y)$,

$$\begin{gathered}
E(Z)=E(f(X, Y))=\sum_{x: y} f(x, y) p_{X: Y}(x, y) \\
E(a X+b Y)=a E(X)+b E(y) \\
E(X-Y)=E^{\prime}(X)+E(Y)
\end{gathered}$$

$\cdot$ Se $X$ e $Y$ sāo independentes:
$$E(X Y)=E(X) E(Y)$$

### Variância e Desvio Padrão $(\sigma)$

$$\begin{gathered}
Var(X)=E\left[(X-E(X))^2\right] \\
Var(X)=E\left(X^2\right)-(E(X))^2 \\
\sigma(X)=\sqrt{Var(X)}
\end{gathered}$$

$\cdot$ Propriedades:
$$\begin{gathered}
Var(a X \mid b)=a^2 Var(X) \\
\sigma(a X+b)=|a| \cdot \sigma(X) \\
Var(b)=0 \\
Var(X+b)-Var(X) \\
Var(a X)=a^2 Var(X)
\end{gathered}$$

$\cdot$  Se $X$ e $Y$ säo independentes:
$$Var(X \mid Y)=Var(X) \text { । } Var(Y)$$

### Desigualdade de Chebyshev

Seja $X$ uma variável aleatória com valor esperado $\mu=E(X)$ e desvio padräo $\sigma(X)$.
Para um intervalo $P, P=\{x \in \mathbb{R} \| x-\mu \mid<k \sigma\}$.
Para qualquer $k>0$, teremos:
$$\begin{gathered}
Pr(X \notin P) \leq \frac{1}{k^2} \\
Pr(\mid X-\mu \geq k \sigma) \leq \frac{1}{k^2} \\
Pr(|X-\mu|<k \sigma) \geq 1-\frac{1}{k^2}
\end{gathered}$$

### Covariância e Correlação $(\rho)$
$$Cov(X, Y)=E(X Y)-E(X) E(Y)$$

$\cdot$ Se $X$ e $Y$ são independentes:
$$\begin{gathered}
Cov(X, Y)=E(X Y)-E(X) E(Y)=0 \\
\rho(X, Y)=\frac{Cov(X, Y)}{\sigma(X) \sigma(Y)}
\end{gathered}$$

$\cdot$ Propriedades de Covariância:

$$\begin{gathered}
Cov(X, Y)=Cov(Y, X) \\
Cov(a X, Y)=a Cov(X, Y) \\
Cov(X+Y, Z)-Cov(X, Z)+Cov(Y, Z) \\
Var(X+Y)-Var(X)+Var(Y)+2 Cov(X, Y) \\
Cov(a X+b, Y)=a Cov(X, Y)
\end{gathered}$$

### Quartis

Qualquer valor $x_2$ onde a função acumulada acerta $q$ ou "passa" por $q$.

$$F\left(x_q^{-}\right) \leq q \leq F\left(x_y\right)$$

- Primeiro Quartil: 0.25
- Segundo Quartil: 0.5 (mediana)
- Terceiro Quartil: 0.75
