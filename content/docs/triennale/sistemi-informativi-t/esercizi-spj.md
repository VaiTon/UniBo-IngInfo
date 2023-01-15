---
title: Esercizi SPJ
---

# Esercizi Select, Project, Join

Corrisponde al **primo esercizio del compito d'esame**.

_es: Per ogni esame in cui il voto è 30, voglio il rispettivo studente_

> ⚠️ Attenzione al **per ogni**, ovvero alla **ricerca di una proprietà universale**.

_es: Studenti che non hanno mai preso 30_

## Push down della selezione

Se in qualsiasi equazione in algebra relazionale si ha una selezione ed un join, posso invertire l'ordine delle operazioni.

{{<katex>}}\sigma*{F_1 \cdot F_2}(R \bowtie S) = \sigma*{F*1}({R}) \bowtie \sigma*{F_2}({S}){{</katex>}}

Ovviamente il procedimento descritto dalla seconda equazione è più efficiente, perché il join è eseguito su relazioni più piccole. Il join è un'operazione molto costosa, quindi è sempre meglio ridurre il numero di tuple coinvolte.

## Irrilevanza dell'ordine del join

{{<katex>}}R \bowtie S = S \bowtie R{{</katex>}}

## Forma canonica

1. Prima tutti i join
2. Poi tutte le selezioni
3. Infine tutte le proiezioni


