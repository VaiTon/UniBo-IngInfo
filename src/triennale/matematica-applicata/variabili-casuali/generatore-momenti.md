---
title: Funzione generatrice dei momenti
---

# Funzione generatrice dei momenti

## Proprietà di riproducibilità delle variabili casuali Binomiali

Siano {{<katex>}}X, Y{{</katex>}} due variabili casuali **Binomiali** indipendenti, tali che:

{{<katex display>}}
\begin{aligned}
X &\sim B(n, p) \\
Y &\sim B(m, p)
\end{aligned}
{{</katex>}}

Allora:

{{<katex display>}}X + Y \sim B(n + m, p){{</katex>}}

#### Dimostrazione

{{<katex>}}\phi_X(t) = (e^tp+q)^n{{</katex>}}
<br>
{{<katex>}}\phi_Y(t) = (e^tp+q)^m{{</katex>}}

Allora:

{{<katex>}}\phi_{X+Y}(t) = \phi_X(t)\cdot\phi_Y(t)= (e^tp+q)^{n+m} {{</katex>}}

