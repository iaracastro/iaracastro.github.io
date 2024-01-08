---
tags: probability
title: Conceitos Iniciais
#published: false
sidebar:
    nav: docs-en
---

### Definições

$\cdot$ Probabilidade: É um modelo num espaço S com elementos associa cada evento a uma probabilidade.

$\cdot$ Espaço Amostral: Conjunto de todos os resultados possíveis de um experimento.

$\cdot$ Eventos Mutuamente excludentes: Seja dois eventos $A$ e $B. A \cup B=\phi$

$\cdot$ Lei da Adição: $\operatorname{Pr}(A \cup B)=\operatorname{Pr}(A)+\operatorname{Pr}(B)-\operatorname{Pr}(A \cap B)$

$\cdot$ Lei da Multiplicação: $\operatorname{Pr}(A \cap B)=\operatorname{Pr}(B \mid A) \cdot \operatorname{Pr}(A)=\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)$

$\cdot$ Probabilidade Condicional: Sejam dois eventos $A$ e $B$ com $\operatorname{Pr}(A) \neq 0$. A probabilidade condicional de $B$ dado $A$ é:
$$
\operatorname{Pr}(B \mid A)=\frac{\operatorname{Pr}(A \cap B)}{\operatorname{Pr}(A)}
$$

$\cdot$ Lei da Probabilidade Total:
$$
\operatorname{Pr}(A)=\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)+\operatorname{Pr}(A \mid \bar{B}) \cdot \operatorname{Pr}(\bar{B})
$$

$\cdot$ Lei da Adição:
$$
\operatorname{Pr}(A \cup B)=\operatorname{Pr}(A)+\operatorname{Pr}(B)-\operatorname{Pr}(A \cap B)
$$

$\cdot$ Lei da Multiplicação:
$$
\operatorname{Pr}(A \cap B)=\operatorname{Pr}(B \mid A) \cdot \operatorname{Pr}(A)=\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)
$$

$\cdot$ Probabilidade Condicional:
Sejam dois eventos $A$ e $B$ com $\operatorname{Pr}(A) \neq 0$. A probabilidade condicional de $B$ dado $A$ é:
$$
\operatorname{Pr}(B \mid A)=\frac{\operatorname{Pr}(A \cap B)}{\operatorname{Pr}(A)}
$$

$\cdot$ Lei da Probabilidade Total:
$$
\operatorname{Pr}(A)=\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)+\operatorname{Pr}(A \mid \bar{B}) \cdot \operatorname{Pr}(\bar{B})
$$

$\cdot$ Teorema de Bayes:
(substituir fórmulas da multiplicação e da probabilidade total na fórmula da probabilidade condicional)
$$
\operatorname{Pr}(B \mid A)=\frac{\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)}{\operatorname{Pr}(A \mid B) \cdot \operatorname{Pr}(B)+\operatorname{Pr}(A \mid \bar{B}) \cdot \operatorname{Pr}(\bar{B})}
$$

