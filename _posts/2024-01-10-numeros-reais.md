---
tags: real-analysis
title: Números Reais
#published: false
sidebar:
    nav: docs-en
---

Isto significa que estão definidas em $\mathbb{R}$ duas operações, chamadas adição e multiplicação, que cumprem certas condições, abaixo especificadas.

A adição faz corresponder a cada par de elementos $x, y \in \mathbb{R}$, sua soma $x+y \in \mathbb{R}$, enquanto a multiplicação associa a esses elementos o seu produto $x \cdot y \in \mathbb{R}$.
Os axiomas a que essas operações obedecem são:

- Associatividade: para quaisquer $x, y, z \in \mathbb{R}$ tem-se $(x+y)+z=x+(y+z)$ $\mathrm{e}(x \cdot y) \cdot z=x \cdot(y \cdot z)$
- Comutatividade: para quaisquer $x, y \in \mathbb{R}$ tem-se $x+y=y+x$ e $x \cdot y=y \cdot x$. Elementos neutros: existem em $\mathbb{R}$ dois elementos distintos 0 e 1 tais que $x+0=x$ e $x \cdot 1=x$ para qualquer $x \in \mathbb{R}$.
- Inversos: todo $x \in \mathbb{R}$ possui um inverso aditivo $-x \in \mathbb{R}$ tal que $x+$ $(-x)=0$ e, se $x \neq 0$, existe também um inverso multiplicativo $x^{-1} \in \mathbb{R}$ tal que $x \cdot x^{-1}=1$.
- Distributividade: para $x, y, z \in \mathbb{R}$ quaisquer, tem-se $x \cdot(y+z)=x \cdot y+x \cdot z$.

#### Desigualdade Triangular (e inversa):
Se $x,y \in \mathbb{R}$:

$$|x+y| \leq |x| + |y|$$

$$|x - y| \geq |x| - |y|$$

$$|x-y| \geq ||x| - |y||$$


### $\mathbb{R}$ é um corpo

Isto significa que existe um subconjunto $\mathbb{R}^{+} \subset \mathbb{R}$, chamado o conjunto dos números reais positivos, que cumpre as seguintes condições:

P1. A soma e o produto de números reais positivos são positivos. Ou seja, $x, y \in \mathbb{R}^{+} \Rightarrow x+y \in \mathbb{R}^{+}$e $x \cdot y \in \mathbb{R}^{+}$. \
P2. Dado $x \in \mathbb{R}$, exatamente uma das três alternativas seguintes ocorre: ou $x=0$, ou $x \in \mathbb{R}^{+}$ou $-x \in \mathbb{R}^{+}$.

Valem as seguintes propriedades da relação de ordem $x < y$ em $\mathbb{R}$ :

- Transitividade: se $x < y$ e $y < z$ então $x < z$.
- Tricotomia: dados $x, y \in \mathbb{R}$, ocorre exatamente uma das alternativas $x=y, x < y$ ou $y < x$.
- Monotonicidade da adição: se $x < y$ então, para todo $z \in \mathbb{R}$, tem-se $x + z < y + z$.
- Monotonicidade da multiplicação: se $x < y$ então, para todo $z>0$ tem-se $x z < y z$. Se, porém, $z<0$ então $x < y$ implica $y z < x z$.

#### Propriedade 

Sejam $a, x, \delta \in \mathbb{R}$. Tem-se $|x-a| < \delta$ se, e somente se, $a-\delta< x < a+\delta$

#### $\mathbb{R}$ é um corpo ordenado completo.

- Diferencia os reais dos racionais.
- Operações usuais (+, . ) 
- Ordem $\leq$ , $<$

### $\mathbb{R}$ não é enumerável

### Limitado Superiormente e Inferiormente
Um conjunto $X \subset \mathbb{R}$ diz-se limitado superiormente quando existe algum $b \in \mathbb{R}$ tal que $x \leq b$ para todo $x \in X$. Neste caso, diz-se que $b$ é uma cota superior de $X$. Analogamente, diz-se que o conjunto $X \subset \mathbb{R}$ é limitado inferiormente quando existe $a \in \mathbb{R}$ tal que $a \leq x$ para todo $x \in X$. O número $a$ chama-se então uma cota inferior de $X$. Se $X$ é

### Supremo e Ínfimo (conjuntos)
Mais explicitamente, $b$ é o supremo de $X$ quando cumpre as duas condições:

- Para todo $x \in X$, tem-se $x \leq b$;
- Se $c \in \mathbb{R}$ é tal que $x \leq c$ para todo $x \in X$ então $b \leq c$. Ou, se $c < b$ então existe $x \in X$ com $c < x$.

#### Propriedades

- $\sup(A + B) = \sup(A) + \sup(B)$ 
- $\inf(A + B) = \inf(A) + \inf(B)$
- Se A é limitado superiormente e $B \subset A$ então $\sup (A) \geq$ $\sup (B)$
- Se A é limitado inferiormente e $B \subset A$ então $\inf (A) \leq$ $\inf (B)$
- Sejam A e B conjuntos limitados de números positivos, então vale $\sup (A \cdot B)=\sup (A) \cdot \sup (B)$
- Sejam A e B conjuntos limitados de números positivos, então vale $\inf (A \cdot B)=\inf (A) \cdot \inf (B)$

Sejam A e B conjuntos limitados de números positivos, então vale $\inf (A \cdot B)=\inf (A) \cdot \inf (B)$

### Supremo e Ínfimo (funções)
Seja uma função limitada $f: V \rightarrow R$.

Definição 1.
$$\sup f:=\sup f(V)=\sup \{f(x) \mid x \in V\}$$

Definição 2.
$$\inf f:=\inf f(V)=\inf \{f(x) \mid x \in V\}$$

Sejam $f, g: V \rightarrow R$ funções limitadas .

#### Propriedades 

- $\sup(f+g) \leq \sup(f) + \sup(g)$
- $\inf(f+g) \geq \inf(f) + \inf(g)$

#### Axioma do supremo
Todo conjunto $A$ $\subseteq$ $\mathbb{R}$ limitado superiormente possui supremo.
- Sup A: menor cota superior de A.
	- sup $A \geq a \; \forall \; a \in A$ 
	- Dado $c \in \mathbb{R}$ tal que $c \geq a \; \forall \; a \in A$, tem-se que $sup(A)$ $\leq \; c$
	- $\forall \epsilon > 0$, existe $a \in A$ tal que: $sup(A) - \epsilon < a \leq sup A$

### Propriedades dos Reais

- Unicidade do elemento neutro da adição: Se $x + \theta = x$, para algum $x \in \mathbb{R}$ então $\theta = 0$

$$x + \theta = \theta + 0$$
$$x + \theta - \theta = \theta - \theta + 0$$
$$x = 0$$

- Unicidade do elemento neutro da multiplicação: Se $x \cdot u = x$ para todo $x \in \mathbb{R}$, então $u = 1$.

Se $x \neq 0$, 
$$x^{-1} \cdot x \cdot u = x^{-1} \cdot x$$
$$1 \cdot u = 1$$
$$y = 1

- x + y = 0, então y = -x

$$x - x + y = 0 + x$$
$$y = x$$

- Se $x \cdot y = 1$, então $y = x^{-1}$

Se $x \cdot y = 1$, $x \neq 0$ e $y \neq 0$, logo, possuem inverso.
$$x^{-1} \cdot x \cdot y = 1 \cdot x^{-1}$$
$$1 \cdot y = 1 \cdot x^{-1}$$
$$y = x^{-1}$$

- Se $(b \cdot d)^{-1} = b^{-1}d^{-1}$

$$(b \cdot d)^{-1} \cdot (b \cdot d) = b^{-1}d^{-1} \cdot (b \cdot d)$$
$$1 = b^{-1}d^{-1} \cdot (b \cdot d)$$

Pela unicidade do inverso, $b^{-1}d^{-1} = (b \cdot d)^{-1}$

- $\frac{a}{b}+\frac{c}{d}=\frac{a d+b c}{b d}$

$$\frac{a}{b}+\frac{c}{d}=\frac{a}{b} \frac{a}{d}+\frac{c}{d} \frac{b}{b}$$
$$=\frac{a d+b c}{b d}$$

- $\left(x^{-1}\right)^{-1}=x$.

Dado que $x \cdot x^{-1}=1$, temos que $x$ é o inverso de $x^{-1}$, isto é $x=\left(x^{-1}\right)^{-1}$.
