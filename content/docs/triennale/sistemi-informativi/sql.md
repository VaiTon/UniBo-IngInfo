---
title: SQL
weight: 2
---
## Data Definition Language

Permette di:

- definire
- modificare
- eliminare

**schemi di relazioni** (tables).

Posso creare inoltre vincoli a livello di:

- singole tuple
- tabelle intere

Posso anche creare nuovi domini.

## `CREATE TABLE`

Si definisce uno schema e viene creata un'istanza vuota.

Sono necessari:

- Almeno un attributo
- Per ogni attributo un dominio ed eventualmente vincoli e default

### Foreign keys

Non posso referenziare un attributo che ANCORA non esiste. Nel caso devo prima creare la tabella senza vincoli e poi aggiungerli via `ALTER TABLE`.

## `SELECT`

## Raggruppamenti

La funzione `AVG` restituisce un numero intero. Per ottenere un numero decimale è necessario effettuare il casting.

## Subquery

### Con operatori di confronto

Gli operatori di confronto possono essere usati solo se la subquery restituisce una sola tupla (subquery scalare).

### Con operatori di aggregazione

Se si utilizzano gli operatori di confronto con una subquery che non restituisce una singola tupla, è necessario specificare in che modo effettuare il _match_.

La forma `IN` equivale a `=ANY`.

### Subquery correlate
