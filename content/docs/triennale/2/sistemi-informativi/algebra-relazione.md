---
title: Algebra relazionale
weight: 1
---

# Algebra relazionale

Il **DML** (Data Manipulation Language) è la parte del linguaggio SQL che permette di eseguire operazioni su relazioni.

## Linguaggi formalmente definiti

- Calcolo relazionale: **dichiarativo**, basato sulla logica dei _predicati del primo ordine_.
- Algebra relazionale: **procedurale**, di tipo algebrico, i cui operandi sono le **relazioni**.

## Operatore: Selezione

| Simbolo | {{<katex>}}\sigma_F{R}{{</katex>}} |
| ------- | ---------------------------------- |

### Caratteristiche

- **Schema:** Lo stesso di {{<katex>}}R{{</katex>}}.
- **Relazione:** Le tuple di {{<katex>}}R{{</katex>}} che soddisfano il predicato {{<katex>}}F{{</katex>}}.

Le tuple sono analizzate una alla volta, e se soddisfano il predicato vengono incluse nella relazione risultante.

### Proprietà

- **Idempotenza:** {{<katex>}}\sigma_F{\sigma_F{R}} = \sigma_F{R}{{</katex>}}

## Operatore: Proiezione

| Simbolo | {{<katex>}}\pi_Y{R}{{</katex>}} |
| ------- | ------------------------------- |

### Caratteristiche

- **Schema:** Solo gli attributi indicati.
- **Relazione:** Le tuple di {{<katex>}}R{{</katex>}} con solo gli attributi indicati.

### Proprietà

- La proiezione **elimina i duplicati**. La **cardinalità** della relazione risultante è sempre minore o uguale a quella di {{<katex>}}R{{</katex>}}.

  > Se si proietta su una superchiave la cardinalità del risultato sarà uguale a quella di {{<katex>}}R{{</katex>}}.

## Operatore: Join naturale

| Simbolo | {{<katex>}}R \bowtie S{{</katex>}} |
| ------- | ---------------------------------- |

### Caratteristiche

- **Schema:** Unione degli schemi delle relazioni coinvolte.
- **Relazione:** Le tuple che hanno gli stessi valori per gli attributi in comune.

### Osservazioni

- Se una tupla di una relazione non ha corrispondenza nella relazione opposta, non viene inserita nella relazione risultante (tupla **dangling**).

### Casi limite

- Se le due relazioni hanno lo stesso schema, la join naturale equivale all'intersezione (se non sono ammessi valori nulli nello schema).
- Se le due relazioni non hanno attributi in comune, la join naturale equivale al prodotto **cartesiano** (a differenza di quest'ultimo non è però ordinato).

### Proprità

- **Idempotenza:** \\(R \bowtie S = S \bowtie R \\)
- **Associatività:** \\((R \bowtie S) \bowtie T = R \bowtie (S \bowtie T) \\)
- **Commutatività:** \\(R \bowtie S = S \bowtie R \\)

## Operatore: Unione

## Operatore: Differenza

## Operatore: Ridenominazione

| Simbolo | \\( \rho\_{Y<-X}{(r)} \\) |
| ------- | ------------------------- |

## Operatore: Divisione

| Simbolo | \\(R \div S\\) |
| ------- | -------------- |

### Caratteristiche

- **Schema:** La differenza tra lo schema di {{<katex>}}R{{</katex>}} e quello di {{<katex>}}S{{</katex>}}.
- **Relazione:** Le tuple di {{<katex>}}R{{</katex>}}, proiettate sullo schema risultante, il cui prodotto cartesiano con {{<katex>}}S{{</katex>}} è contenuto in {{<katex>}}R{{</katex>}}.

\\[R \div S = A, \quad A \cdot S \subseteq R \\]

La divisione potrebbe quindi essere vista come l'operazione inversa della join naturale.

> ⚠️ E' opportuno considerare che, se è necessario cercare "per ognuno" qualcosa di diverso (e non "per tutti" la stessa cosa), la divisione non è sempre la soluzione.
