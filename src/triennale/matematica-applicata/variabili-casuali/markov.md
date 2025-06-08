---
title: Disuguaglianza di Markov
---

# Disuguaglianza di Markov

## Teorema

Data una variabile casuale {{<katex>}}X \ge 0{{</katex>}} e data {{<katex>}}a \in \mathbb R{{</katex>}}, vale:

{{<katex display>}}
    P(X \ge a) \le \frac {E[X]}{a}
{{</katex>}}

Ovvero, riusciamo a stimare {{<katex>}}P(X \ge a){{</katex>}} attraverso il suo **valor medio**.

## Osservazione

{{<katex>}}\displaystyle\frac {E[X]} a \lt 1{{</katex>}}, perchè altrimenti il risultato non è significativo.

{{<hint warning>}}
Ricorda che la probabilità è sempre minore di 1!
{{</hint>}}

## Dimostrazione

La dimostrazione è effettuata per il caso continuo, ma è facile estenderla al caso discreto.

### Caso continuo

Supponiamo che {{<katex>}}X{{</katex>}} sia una variabile casuale continua con densità di probabilità {{<katex>}}f{{</katex>}} e che {{<katex>}}a \gt 0{{</katex>}}.

{{<katex display>}}
\begin{aligned}

E[X] \overset{\text{per def}}{=} & \int_{\mathbb R} x f(x) dx \quad
\overbrace{=}^{x \ge 0} \int_{0}^{\infty} x f(x) dx
\\
=& \int_0^a x f(x) dx + \int_a^{\infty} x f(x) dx \ge \int_a^{\infty} x f(x) dx \\
\underbrace{\ge}_{x \ge a}&\int_a^{\infty} a f(x) dx = a \underbrace{\int_a^{\infty} f(x) dx}_{\text{definizione di } P(X \ge a)}
\\
=& \quad \bold{a \cdot P(X \ge a)}

\end{aligned}
{{</katex>}}



