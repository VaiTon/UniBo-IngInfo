---
title: Generazione di numeri casuali
---

{{<katex>}}{{</katex>}}

# Generazione di numeri casuali

## Introduzione

Esistono tre modi per generare dei numeri casuali:

1. Sequenze di numeri casuali ottenuti dall'osservazione di fenomeni fisici (es. decadimento radioattivo).
2. Sequenze di numeri pseudo-casuali ottenuti da algoritmi deterministici (es. generatore di numeri pseudo-casuali).
3. Sequenze di numeri **quasicasuali**, ovvero distribuiti uniformemente ma non del tutto randomici.

## Caratteristiche delle sequenze di numeri pseudo-casuali

1. Buona distribuzione: casualità + uniformità.
2. Periodo lungo: tutte le sequenze sono periodiche, si cerca però una sequenza con il periodo più lungo possibile.
3. Ripetibilità: se inizio con lo stesso _seme_, ottengo la stessa sequenza.

## Tipologie

1. Generatori lineari congrenziali (anche detti moltiplicativi)

   Sia \\(S_0\\) il seme (un numero "grande").

   \\[
   \begin{aligned}
   S_1 &= (aS_0 + c) \mod m \\\
   S_2 &= (aS_1 + c) \mod m \\\
   S_{i+1} &= (aS_i + c) \mod m
   \end{aligned}
   \\]

   con \\(m >> 1 \\) e il valore \\(V_i\\) è dato da:
   \\[
   V_i = \frac{S_i}{m}
   \\]

2. Generatori di fibonacci

    \\[
    \begin{aligned}
        S_K &= (S_{K-1} + S_{K-2}) \mod m \qquad \text{(no lag)} \\\
        S_K &= (S_{K-p} + S_{K-q}) \mod m \qquad \text{(con lag)}
    \end{aligned}
    \\]

### Esempio: Merseene Twister

Il generatore di numeri pseudo-casuali più utilizzato è il [Mersenne Twister](https://en.wikipedia.org/wiki/Mersenne_Twister).

Il generatore è basato su un generatore lineare congrezionale con:
- \\(m = 2^{19937} - 1\\)
- \\(a = 1812433253\\)
