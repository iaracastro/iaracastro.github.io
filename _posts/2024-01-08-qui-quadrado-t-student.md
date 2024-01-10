---
tags: probability
title: Qui-Quadrado e T-Student
#published: false
sidebar:
    nav: docs-en
---

## Distribuição Qui-Quadrado

A distribuição χ2 ou qui-quadrado é uma das distribuições mais utilizadas em estatística inferencial, principalmente para realizar testes de χ2. Este teste serve para avaliar quantitativamente a relação entre o resultado de um experimento e a distribuição esperada para o fenômeno. Isto é, ele nos diz com quanta certeza os valores observados podem ser aceitos como regidos pela teoria em questão. Muitos outros testes de hipótese usam, também, a distribuição $\chi^2$.

$$Y \sim \chi^2(n)$$

$\mathrm{n}$ : graus de liberdade

$$\begin{gathered}
f(y)=\frac{1}{\Gamma\left(\frac{n}{2}\right) 2^{n / 2}} y^{\frac{n}{2}-1 e^{-y / 2}}, \quad y>0 \\
E(Y)=n \\
\text{ Var }(Y)=2 n
\end{gathered}$$

## Distribuição T-student

A distribuição $t$ é uma distribuição de probabilidade absolutamente contínua, simétrica e campaniforme, o único parâmetro que a caracteriza esta família é o número de graus de liberdade. A função densidade de probabilidade da $t$ detém caudas mais pesadas que a distribuição normal quando 
$n$ é pequeno e a medida que $n$ cresce, a distribuição t de Student se aproxima da normal.

$$T \sim t(n)$$

$$\begin{gathered}
f(t)=T \text{ Den }(t ; n)=\frac{\Gamma\left(\frac{n + 1}{2}\right)}{\Gamma\left(\frac{n}{2}\right) \sqrt{\pi n}}\left(1+\frac{t^2}{n}\right)^{-(n-1) / 2} \\
E(T)=0, \quad n \geq 2 \\
\text{ Var }(T)=\frac{n}{n-2}, \quad n \geq 3
\end{gathered}$$

$$Z \sim N(0,1) \text { e } X \sim \chi^2(n)$$

$$T=\frac{Z}{\sqrt{X / n}}$$

é chamada de $t$ de Student com $n$ graus de liberdade. $T \sim t(n)$
