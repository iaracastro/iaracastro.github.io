---
tags: probability
title: Somas e Médias de V.A
#published: false
sidebar:
    nav: docs-en
---

## Definições
Seja $\left(X_1, X_2, \ldots, X_*\right)$ um conjunto de variáveis aleatórias de uma distribuição $X$. Definimos:

$$\begin{gathered}
S_n=X_1+X_2+\ldots+X_n \\
\bar{X}=\frac{S_n}{n}=\frac{X_1-X_2+\ldots+X_n}{n}
\end{gathered}$$

## Propriedades da Distribuição Normal
Se $X_1 \sim N\left(\mu_1, \sigma_1^2\right)$ e $X_2 \sim N\left(\mu_2, \sigma_2^2\right)$ são independentes, entấo qualquer combinaçẫo linear: $X=a X_1+b X_2$ também terá distribuição normal.

$$a X_1+b X_2 \sim N\left(a \mu_1+b \mu_2, a^2 \sigma_1^2+b^2 \sigma_2^2\right)$$

Se $X_i \sim N\left(\mu, \text{sigman}^2\right)$

$$\begin{gathered}
S_{n^c} \sim N\left(n \mu, n \sigma^2\right) \\
X \sim N\left(\mu, \frac{\sigma^2}{n}\right)
\end{gathered}$$

Se $X_1, X_2, \ldots, X_n$ säo i.i.d $\text{com} X_i \sim N\left(\mu, \sigma^2\right)$

$$\begin{aligned}
& \frac{S_{v_i}-n \mu}{\sqrt{n} \sigma} \sim N(0,1) \\
& \frac{\bar{X}-\mu}{\sigma / \sqrt{n}} \sim N(0,1)
\end{aligned}$$

- Propriedades para $S_n$

$$\begin{gathered}
E\left(S_n\right)=n \mu \\
\text{Var}\left(S_n\right)=n \sigma^2 \\
\sigma\left(S_n\right)=\sqrt{n} \tau
\end{gathered}$$

- Propriedades para $\bar{X}$

$$\begin{gathered}
E(\bar{X})=\mu \\
\operatorname{Var}(\bar{X})=\frac{\sigma^2}{n} \\
\sigma(X)=\frac{\sigma}{\sqrt{n}}
\end{gathered}$$

## Desigualdade de Chebyshev
Se $E(X)=\mu$ e $\sigma(X)=\sigma$, entāo para qualquer $k \circlearrowleft(0$ :

$$Pr(|x-\mu|>k \sigma) \leq \frac{1}{k^2}$$

## Lei dos Grandes Números (LGN)
Quanto maior o número n de variáveis aleatórias, $E(\bar{X})$ permanece constante, mas $\operatorname{Var}(\bar{X})$ se aproxima de 0 . Entäo a distribuiçäo de $\bar{X}$ fica cada vez mais concentrada em $E(X)$.

Para qualquer $c>0$ fixo:

$$Pr(|\bar{X}-\mu| \geq \epsilon) \rightarrow 0$$

quando $n \rightarrow \infty$

$$Pr(|\bar{X}-\mu|<\epsilon) \rightarrow 1$$

Colocando $\bar{X}$ na desigualdade de Chebyshev e substituindo $E(\bar{X})$ por $E(X)=\mu$ e $\sigma(\bar{X})$ por $\sigma / \sqrt{n}$

$$0<Pr\left(\left|\bar{X}-\mu \geq \frac{k \sigma}{\sqrt{n}}\right|\right) \leq \frac{1}{k^2}$$

Escolhendo $k=\epsilon \sqrt{n} / \sigma$

$$0<Pr(\mid \bar{X}-\mu \geq \epsilon) \leq \frac{\sigma^2}{n \epsilon^2}$$

## Teorema Central do Limite (TCL)

Sejam $X_1, X_2, \ldots, X_{\mathrm{r}}$ amostras independentes de uma densidade com valor esperado $\mu \mathrm{e}$ variância $\sigma^2$

$$\begin{gathered}
X^* = \sqrt{n} \frac{\bar{X}-\mu}{\sigma}=\frac{S_n-n \mu}{\sigma \sqrt{n}} \\
\lim _{n \rightarrow \infty} \text{ Or } \left(a \leq X^* \leq b\right)=\int_a^b \phi(x) d x
\end{gathered}$$

--- 

$$X \sim \text{ Bin }(n, p) \Rightarrow Pr(a \leq X \leq b) \simeq \text{ NormalDist }\left(\frac{b+\frac{1}{2}-n p}{\sqrt{n p q}}\right)-\text{NormalDist}\left(\frac{a-\frac{1}{2}-n p}{\sqrt{\pi p q}}\right)$$

- Se $n$ é grande e $X \sim \text{ Neg } \text{ Bin }(n, p)$, então $X \approx N\left(\frac{n}{p}, \frac{n q}{p^2}\right)$

- Se $\lambda$ é grande e $X \sim \text{Poi}(\lambda)$, então $X \approx N(\lambda, \lambda)$

- Se $n$ é grande e $X \sim \text{Gamma}(n, \lambda)$, então $X \approx N\left(\frac{n}{\lambda}, \frac{n}{\lambda^2}\right)$
