---
title: Esercizio 1
weight: 1
---

# Guida per l'esercizio 1

## Parole chiavi e operatori

{{<hint warning>}}
⚠️ Da prendere con le pinze
{{</hint>}}

Qui sotto una tabella delle parole chiavi legate alle operazioni da utilizzare:

| Parole chiavi       | Operazione                                      |
| ------------------- | ----------------------------------------------- |
| mai, nessuno        | [sottrazione]({{<ref "riassunto#differenza">}}) |
| tutti quelli che... | [divisione]({{<ref "riassunto#divisione">}})    |

## Self join

Utilizzando un esempio...

`i furgoni che hanno fatto almeno 2 o più soste`

```text
+-------+
| Soste +--> Ridenom(attr2<-attr1) -+
+-------+                           |
                                    v
                                    JOIN ---> Seleziona(attr1 <> attr2)
                                    ^
+-------+                           |
| Soste +---------------------------+
+-------+
```
