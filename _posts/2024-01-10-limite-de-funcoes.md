---
tags: real-analysis
title: Limite de FunçÕes
#published: false
sidebar:
    nav: docs-en
---

Definição: Sejam $X \subset \mathbb{R}$ um conjunto de números reais, $f: X \rightarrow \mathbb{R}$ uma função real cujo domínio é $X$ e $a \in X^{\prime}$ um ponto de acumulação do conjunto $X$. Dizse que o número real $L$ é limite de $f(x)$ quando $x$ tende para $a$, e escrevese $\lim _{x \rightarrow a} f(x)=L$, quando, para todo $\varepsilon>0$ dado arbitrariamente, pode-se obter $\delta>0$ tal que se tem 

$$|f(x)-L|<\varepsilon$$ 

sempre que 

$$x \in X \text{ e } 0<|x-a|<\delta$$

---

$$\lim _{x \rightarrow a} f(x)=L \; \equiv \; \forall \varepsilon>0 \exists \delta>0 ; x \in X, 0<|x-a|<\delta \Rightarrow|f(x)-L|<\varepsilon$$

Em outras palavras, $\lim _{x \rightarrow a} f(x)=L$ quer dizer que se pode tornar $f(x)$ tão próximo de $L$ quanto se queira desde que se tome $x \in X$ suficientemente próximo, porém diferente de $a$. 

## Teoremas

1. Sejam $f, g: X \rightarrow \mathbb{R}, a \in X^{\prime}, \lim _{x \rightarrow a} f(x)=L$ e $\lim _{x \rightarrow a} g(x)$ $=M$. Se $L < M$ então existe $\delta>0$ tal que $f(x) < g(x)$ para todo $x \in X$ com

$$0<|x-a|<\delta$$

2. Se $\lim_{x \rightarrow a} f(x)=L < M$ então existe $\delta < 0$ tal que $f(x) < M$ para todo $x \in X$ com

$$0<|x-a|<\delta$$

3. Sejam $\lim_{x \rightarrow a} f(x)=L$ e $\lim _{x \rightarrow a} g(x)=M$. Se $f(x) \leq$ $g(x)$ para todo $x \in X-\{a\}$ então $L \leq M$.

4. **(Teorema do sanduíche)** Sejam $f, g, h: X \rightarrow \mathbb{R}, a \in$ $X^{\prime}$ e $\lim _{x \rightarrow a} f(x)=\lim _{x \rightarrow a} g(x)=L$. Se $f(x) \leq h(x) \leq g(x)$ para todo $x \in X-\{a\}$ então $\lim _{x \rightarrow a} h(x)=L$.

5. Sejam $f: X \rightarrow \mathbb{R}$ e $a \in X^{\prime}$. A fim de que seja $\lim _{x \rightarrow a} f(x)=L$ é necessário e suficiente que, para toda seqüência de pontos $x_n \in X-\{a\}$ com $\lim x_n=a$, tenha-se $\lim f\left(x_n\right)=L$.

6. **(Unicidade do limite)** Sejam $f: X \rightarrow \mathbb{R}$ e $a \in X^{\prime}$. Se $\lim_{x \rightarrow a} f(x)=L e \lim_{x \rightarrow a} f(x)=M$ então $L=M$.

## Operações com Limites

Sejam $f, g: X \rightarrow \mathbb{R}, a \in X^{\prime}$, com $\lim _{x \rightarrow a} f(x)=L$ e $\lim _{x \rightarrow a} g(x)=M$. Então

$$\begin{aligned}
& \lim _{x \rightarrow a}[f(x) \pm g(x)]=L \pm M ; \\
& \lim _{x \rightarrow a}[f(x) \cdot g(x)]=\dot{L} \cdot M ; \\
& \lim _{x \rightarrow a} \frac{f(x)}{g(x)}=\frac{L}{M}, \text { se } M \neq 0 .
\end{aligned}$$

- Se $\lim _{x \rightarrow a} f(x)=0$ e $g$ é limitada numa vizinhança de $a$, tem-se $\lim _{x \rightarrow a}[f(x) \cdot g(x)]=0$.

## Exemplos

- $\lim _{x \rightarrow 0}(\text{sen} x / x)=1$
- $\lim _{x \rightarrow 0}\left(e^x-1\right) / x=1$

## Limites Laterais

L é **limite à direita** de $f(x)$ quando:
$$\lim_{x\rightarrow a^{+}} f(x) = L$$
$\forall \epsilon>0$, existe $\delta>0$ tal que:
$$0 < x - a <\delta \Rightarrow|f(x) - L| < \epsilon$$


L é **limite à esquerda** de $f(x)$ quando:
$$\lim_{x\rightarrow a^{-}} f(x) = L$$
$\forall \epsilon>0$, existe $\delta>0$ tal que:
$$0 < a-x < \delta \Rightarrow |f(x) - L| < \epsilon$$

### Existência de Limite

Existe $\lim_{x \rightarrow a} f(x)=L$ se, e somente se, existem e são iguais os limites laterais:

$$\lim_{x \rightarrow a+} f(x)=\lim _{x \rightarrow a-} f(x)=L$$

## Limite de Função Infinita (L)

$f:I\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow \infty} f(x) = L$ se:
Para todo $\epsilon > 0$, existe $\alpha > 0$ tal que $\forall x > \alpha$
$$|f(x) - L| < \epsilon$$

$f:I\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow -\infty} f(x) = L$ se:
Para todo $\epsilon > 0$, existe $\alpha < 0$ tal que $\forall x < \alpha$
$$|f(x) - L| < \epsilon$$

## Limite de Função Infinita ($\pm \infty$)
$f:\mathbb{R}\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow \infty} f(x) = +\infty$ se:
Para todo $A > 0$, existe $\alpha > 0$ tal que $\forall x > \alpha$
$$f(x) > A$$

Analogamente,
$f:\mathbb{R}\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow -\infty} f(x) = +\infty$ se:
Para todo $A > 0$, existe $\alpha < 0$ tal que $\forall x < \alpha$
$$f(x) > A$$

---
$f:\mathbb{R}\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow \infty} f(x) = -\infty$ se:
Para todo $A < 0$, existe $\alpha > 0$ tal que $\forall x > \alpha$
$$f(x) < A$$

$f:\mathbb{R}\rightarrow \mathbb{R}$. Dizemos que $\lim_{x \rightarrow -\infty} f(x) = -\infty$ se:
Para todo $A < 0$, existe $\alpha < 0$ tal que $\forall x < \alpha$
$$f(x) < A$$
