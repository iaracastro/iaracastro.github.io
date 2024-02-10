---
tags: real-analysis
title: Séries de Taylor
#published: false
sidebar:
    nav: docs-en
---

Quando a série de potências $\sum a_n\left(x-x_0\right)^n$ tem raio de convergência $r>0$, diz-se que ela é a série de Taylor, em torno do ponto $x_0$, da função $f:\left(x_0-r, x_0+r\right) \rightarrow \mathbb{R}$, definida por $f(x)=\sum a_n\left(x-x_0\right)^n$. Esta denominação se deve ao fato de que a soma dos primeiros $n+1$ termos desta série constitui o polinômio de Taylor de ordem $n$ de $f$ no ponto $x_0$. 

### Exemplos

1. **Funções seno e cosseno**: Suas séries de Taylor em torno do ponto $x=0$ são

$$\sin x=x-\frac{x^3}{3 !}+\frac{x^5}{5 !}-\cdots$$

$$\cos x=1-\frac{x^2}{2 !}+\frac{x^4}{4 !}-\cdots$$

em virtude da própria definição dessas funções.

2. **Função** $1 /(1-x)$: A série de potências $1+x+x^2+\cdots$ é uma série geométrica. Ela converge para a soma $1 /(1-x)$ quando

$$|x|<1$$ 

e diverge quando 

$$|x| \geq 1$$

Logo é a série de Taylor da função $f:(-1,1) \rightarrow \mathbb{R}$, definida por $f(x)=$ $1 /(1-x)$.

3. **Função exponencial**

A série $\sum_{n=0}^{\infty} x^n / n$ ! converge para todo $x \in \mathbb{R}$, logo a função $f: \mathbb{R} \rightarrow \mathbb{R}$, definida por $f(x)=\sum_{n=0}^{\infty} x^n / n$ !, é de classe $C^{\infty}$. Derivando termo a termo, vemos que $f^{\prime}(x)=f(x)$. Como $f(0)=1$, segue-se do Teorema 10, Capítulo 11, que $f(x)=e^x$ para todo $x \in \mathbb{R}$. Portanto

$$e^x=1+x+\frac{x^2}{2 !}+\frac{x^3}{3 !}+\cdots$$

4. **Função logaritmo**

Como $\log x$ não tem sentido para $x=0$, consideraremos a função $\log (1+x)$, definida para todo $x>-1$. Por definição, $\log (1+x)=$ $\int_0^x d t /(1+t)$. Integrando termo a termo a série de Taylor de $1 /(1+x)$, vista cima, obtemos

$$\log (1+x)=x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}+\cdots=\sum_{n=1}^{\infty}(-1)^{n+1} \frac{x^n}{n},$$

série de Taylor de $\log (1+x)$, convergente no intervalo aberto $(-1,1)$, pois 1 é seu raio de convergência.

5. **Função Arctg**
