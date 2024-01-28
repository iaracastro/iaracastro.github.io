---
tags: real-analysis
title: Derivadas de Funções
#published: false
sidebar:
    nav: docs-en
---

## Definição 

Sejam $f: X \rightarrow \mathbb{R}$ e $a \in X \cap X^{\prime}$. A derivada da função $f$ no ponto $a$ é o limite

$$f^{\prime}(a)=\lim _{x \rightarrow a} \frac{f(x)-f(a)}{x-a}=\lim _{h \rightarrow 0} \frac{f(a+h)-f(a)}{h}$$

Bem entendido, o limite acima pode existir ou não. Se existir, diz-se que **$f$ é derivável no ponto $a$**. 

- Quando existe a derivada $f^{\prime}(x) \mathrm{em}$ todos os pontos $x \in X \cap X^{\prime}$ diz-se que a função $f: X \rightarrow \mathbb{R}$ é derivável no conjunto $X$ e obtém-se uma nova função $f^{\prime}: X \cap X^{\prime} \rightarrow \mathbb{R}, x \mapsto f^{\prime}(x)$, chamada a função derivada de $f$. 

## Classe 

Se $f^{\prime}$ é contínua, diz-se que $f$ é $d e$ classe $C^1$.

## Derivadas Sucessivas
Dizemos que uma função $f:I \rightarrow \mathbb{R}$, $I$ intervalo. Diremos que $f$ é $k$ vezes derivável em $I$ se existem as derivadas sucessivas $f', (f')', ((f')')',...$ $k$ vezes.


## Operações para $f$ e $g$ deriváveis
$f$ e $g$ $: I \rightarrow \mathbb{R}$ deriváveis.

- $f+g$ é derivável $$(f+g)'(x) = f'(x) + g'(x)$$
- $f \cdot g$ é derivável
$$(f \cdot g)'(x) = f'(x)g(x) + f(x)g'(x)$$

- $(1/f)'$
$$\left(\frac{1}{f}\right)' = \frac{-f'}{f^2}$$
- $(f/g)'$
$$\left(\frac{f}{g}\right)' = \frac{f'g - fg'}{g^2}$$
- **(Regra da Cadeia)** Seja $f: I -> j$ derivável e $g: j -> \mathbb{R}$ derivável, temos:
$$(g . f)(x) := g(f(x))$$
$$(g . f)'(x) := g'(f(x)) \cdot f'(x)$$

## Ponto Crítico

Ponto crítico é um ponto onde a derivada se anula.

- Nem sempre um ponto crítico é ponto de máximo ou mínimo globais.

## Ponto de Máximo e Mínimo Local
Seja $f:I\rightarrow \mathbb{R}$ derivável e $c \in I$

Definição 1: \
Existe $\delta>0$ tal que se $(c-\delta, c+\delta) \subset I$ e $f(x) \leq f(c)$, então sempre que $x \in (c-\delta, c+\delta)$; diremos que $c$ é um máximo local de $f$.

Definição 2: \
$c$ é um ponto de máximo (ou mínimo) local se existe $\delta > 0$ tal que $x \in X$,
$$|x-c| < \delta\Rightarrow f(x) \leq f(c)$$

---

Se temos um ponto crítico $d \in (a,b)$ tal que:
- se $g''(d) < 0$, então d é ponto de máximo local.
- se $g''(d) > 0$, então $d$ é ponto de mínimo local.

## Mínimo e Máximo Absoluto

Quando $a \in X$ é tal que $f(a) \leq f(x)$ para todo $x \in X$, diz-se que $a$ é um ponto de mínimo absoluto para a função $f:X \rightarrow \mathbb{R}$. 

Se vale $f(a) \geq f(x)$ para todo $x \in X$ diz-se que $a$ é ponto de máximo absoluto.

## Teoremas

### Teorema do Valor Médio

Seja $f:[a,b]\rightarrow \mathbb{R}$ contínua e derivável em $(a,b)$
Existe $c \in (a,b)$ t.q. $$f'(c) = \frac{f(b) - f(a)}{b-a}$$

### Teorema de Rolle

$g:[a,b]\rightarrow \mathbb{R}$ derivável tal que $g(a) = g(b)$ então existe $c \in (a,b)$ tal que:
$g'(c) = 0$

### Teorema Fundamental do Cálculo
Seja $f:[a,b]\rightarrow \mathbb{R}$ integrável e contínua. Para qualquer $c \in [a,b]$ então $F$ é derivável em $c$ e $F'(c) = f(c)$

$F(x) = \int_a^x{f} \quad$ satisfaz $F'(x) = f(x)$ para todo $x \in [a,b]$

- Quando $f$ é contínua, o Teorema Fundamental do Cálculo mostra que $f$ possui primitiva $F(x) = \int_a^b{f}$.

$$\int_a^b f = F(b) - F(a)$$

---

$$g(x) = g(a) + \int_a^x g'(t)dt$$

### Operações com Integrais
$$\int_a^b f(x) dx = -\int_b^a f(x)dx$$
$$\int_{t_0}^{t_1} f(x) dx + \int_{t_1}^{t_2} f(x)dx = \int_{t_0}^{t_2} f(x)dx$$
$$\int_{b}^a f(x) - \int_{b}^c f(x) = -\int_{a}^b f(x) - \int_{b}^c f(x) = - \left(\int_{a}^b f(x) + \int_{b}^c f(x)\right) = - \left(\int_{a}^c f(x)\right)$$

### Série de Taylor
$$f(x)= T^n_{c,f}(x) := \sum_{j=0}^{n} \frac{f^{(j)(c)}}{j!}(x-c)^j = f(c) + f'(c)(x-c) + \frac{f^{''}(c)}{2!}(x-c)^2+...+\frac{f^{(n)}}{n!}(x-c)^n$$

### Teorema de Darboux
Seja $f:[a,b] \rightarrow \mathbb{R}$ derivável. Se $f'(a) < d < f'(b)$, então existe $c \in (a,b)$, tal que $f'(c) = d$

## Função Localmente Constante
Definição: $\forall x_0 \in (a,b)$ existe tal que $f$  é constante em $(x_0 - \delta, x_0 + \delta)$.
$f'(x) = 0 \; \forall x_0 \in (a,b)$

- Seja $f:I \rightarrow \mathbb{R}$ função localmente constante, então $f$ é constante.


## Função (estritamente) Crescente e Decrescente
Seja $g:I \rightarrow \mathbb{R}$ função derivável.

- Se $g'(x) \geq 0$ para todo $x \in I$ então $g$ é crescente.
- Se $g'(x) > 0$ para todo $x \in I$ então $g$ é estritamente crescente.
- Se $g'(x) \leq 0$ para todo $x \in I$, então $g$ é decrescente.
- Se $g'(x) < 0$ para todo $x \in I$ então $g$ é estritamente decrescente.

Seja $f:I\rightarrow\mathbb{R}$ função inversível.

- Uma função $f$ é dita crescente se para $x_1 < x_2$, tem-se $f(x_1) \leq f(x_2)$.
- Uma função $f$ é dita decrescente se para $x_1 < x_2$, tem-se $f(x_1) \geq f(x_2)$.
- Uma função $f$ é dita estritamente crescente se para $x_1 < x_2$, tem-se $f(x_1) < f(x_2)$.
- Uma função $f$ é dita estritamente decrescente se para $x_1 < x_2$, tem-se $f(x_1) > f(x_2)$.

Para uma função ser inversível, é suficiente que a função seja estritamente crescente ou estritamente decrescente em seu domínio.

- $f$ é estritamente crescente $\Rightarrow$ $f$ é inversível.
- $f$ é estritamente decrescente $\Rightarrow$ $f$ é inversível.

## Raízes de um Polinômio
Teorema: Um polinômio de grau $k \in \mathbb{N}$ possui no máximo $k$ raízes.

 
### Prova

Por indução: Caso base $k=1$, \
O polinômio é da forma: $p(x) = \alpha x + \beta$, portanto, possui 1 raiz. \

Suponhamos a afirmativa válida para polinômios de grau k tenham k raízes; Vamos provar que polinômios de grau $k+1$, possuem no máximo $k+1$ raízes.
Consideramos então que o polinômio $q(x)$ de grau $k+1$; se possuir pelo menos $k+2$ raízes $a_1<a_2,...<a_{k+2}$, Pelo Teorema de Rolle, entre 2 raízes consecutivas existe um ponto onde $q'(x)$ se anula, então $q'(x)$ possui uma raiz em cada intervalo $(a_j, a_{j+1})$. Mas $q'(x)$ é polinômio de grau $k$, absurdo.

## $f$ estritamente convexa para cima (baixo)

Seja $I \subset \mathbb{R}$ um intervalo. Uma função $f: I \rightarrow \mathbb{R}$ chama-se convexa quando seu gráfico se situa abaixo de qualquer de suas secantes. Em termos precisos, a convexidade de $f$ se exprime assim: dado $f:[a,b] \rightarrow \mathbb{R}$,
$f(x) \leq f(a) + \frac{f(b) - f(a)}{b - a}(x-a)$

Para quaisquer $a < x < b$

### Teorema f duas vezes derivável

Uma função $f: I \rightarrow \mathbb{R}$, duas vezes derivável no intervalo $I$, é convexa se, e somente se, $f^{\prime \prime}(x) \geq 0$ para todo $x \in I$.

### Propriedades

- $g$ é estritamente convexa para cima $\Rightarrow$ $g'$ é estritamente crescente.
- $g$ é estritamente convexa para baixo $\Rightarrow$ $g'$ é estritamente decrescente.

### Afirmações

As seguintes afirmações sobre a função $f: I \rightarrow \mathbb{R}$, derivável no intervalo $I$, são equivalentes:

(1) $f$ é convexa. \
(2) A derivada $f^{\prime}: I \rightarrow \mathbb{R}$ é monótona não-decrescente. \
(3) Para quaisquer $a, x \in I$ tem-se $f(x) \geq f(a)+f^{\prime}(a)(x-a)$, ou seja, o gráfico de $f$ está situado acima de qualquer de suas tangentes.
