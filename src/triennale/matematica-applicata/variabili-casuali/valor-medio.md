---
titolo: Valore medio
---
# Valor medio di una variabile casuale

Il **valor medio** di una variabile casuale, anche detto **valore
atteso, media teorica o speranza matematica** è definito in questo
modo:

{{<katex display>}}

E[X] = \begin{cases}
\displaystyle\sum_{k=1}^{n}{x_k \cdot p(x_k)} \quad \text{se } X \text{ discreta, }X \in \{x_1, ... x_n\}\\
\displaystyle\int_{\mathbb{R}}{x \cdot f(x) dx} \quad \text{se } X \text{ continua}
\end{cases}

{{</katex>}}

### Proprietà

#### Proprietà 1.

Se *Y* = *h*(*X*), con *X* variabile casuale nota, vale:

{{<katex display>}}

E[Y] = E[h(X)] = \begin{cases}
\displaystyle\sum{k=1}^n{h(x_k) \cdot p(x_k)}\quad &\text{se } X \text{ discreta, }X \in \{x_1, ... x_n\} \\\
\displaystyle\int_{\mathbb{R}}{h(x) \cdot f(x) dx} \quad &\text{se } X \text{ continua}
\end{cases}

{{</katex>}}

#### Proprietà 2.

*Caso particolare della 1.* Se \\(Y = \alpha X+ \beta\\), con
{{<katex>}}\alpha \in \mathbb{R}, \beta \in \mathbb R{{</katex>}}

{{<katex>}}E[Y] = \alpha E[X] + \beta{{</katex>}}

##### Dimostrazione

Sia {{<katex>}}X{{</katex>}} una variabile casuale discreta, con {{<katex>}}X \in \{x_1, x_2, ..., x_n\}{{</katex>}}

{{<katex display>}}

\begin{aligned}
E[X] &= \sum_{k=1}^{m}{h(x_k) \cdot p(x_k)} = \\
&= \sum_{k=1}^{m}{(\alpha x_k + \beta) \cdot p(x_k)} = \\
&= \alpha \underbrace{\sum_{k=1}^{m}{x_k \cdot p(x_k)}}_{E[X] \text{ per definizione}} + \beta \overbrace{\sum_{k=1}^{m}{p(x_k)}}^{=1 \text{ (prop. funzioni di massa)}} = \alpha E[X] + \beta
\end{aligned}

{{</katex>}}

In maniera simile si dimostra il caso continuo.

#### Proprietà 3.

Se
{{<katex>}}Z = g(X,Y){{</katex>}},
con
{{<katex>}}X, Y{{</katex>}}
variabili casuale note, vale:

{{<katex>}}
E[Z]  =
\begin{cases}
    \displaystyle\sum_{k=1}^m \sum_{j=1}^n g(x_k, y_j) \cdot p(x_k, y_j) \quad
&\text{se } X,y \text{ discrete} \\\
\displaystyle\iint_{\mathbb{R^2}}{g(x,y) \cdot f(x,y) dx dy} \quad
&\text{se } X,Y \text{ continue}
\end{cases}
{{</katex>}}


#### Proprietà 4
Date {{<katex>}}X, Y{{</katex>}} variabili casuali, vale:
{{<katex display>}}E[X+Y] = E[X] + E[Y]{{</katex>}}

## Valor medio di una Bernoulliana

{{<katex>}}X \sim Be(p){{</katex>}}
<br>
{{<katex>}}
X = \begin{cases}
1 \\
0 \\
\end{cases}
{{</katex>}}

{{<katex>}}
p(1) = p \\
p(0) = 1 − p = q
{{</katex>}}

<br>

{{<katex display>}}
E[x] = \underbrace{\sum_{k=1}^m x_k p(x_k)}_{\text{definizione di valor medio}} = 0 \cdot p(0) + 1 \cdot p(1) = 1 \cdot p = p
{{</katex>}}

## Valor medio di una binomiale

## Momento *n*-esimo di una variabile casuale

Se esiste, si definisce il **momento *n*-esimo** di una variabile casuale
{{<katex>}}X{{</katex>}} come:

{{<katex display>}}
E[X^n]
{{</katex>}}

- 0-esimo momento = 1
- 1 momento = {{<katex>}}E[X]{{</katex>}} = valor medio.

Il **valor medio** è definito come il **primo momento**.
