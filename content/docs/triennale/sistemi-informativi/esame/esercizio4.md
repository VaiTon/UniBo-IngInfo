---
title: Esercizio 4
---

# Guida per l'esercizio 4

Questa pagina è una checklist delle cose da fare / non fare per l'esercizio 4 (aggiornata al 2022).

## Attributi compositi

### Attributo composito come identificatore

Se l'**attributo composito è utilizzato come identificatore** è necessario che sia univoco.

E' necessario inserire un trigger `BEFORE INSERT` che controlli che non esistano altre tuple con la stessa combinazione di sotto-attributi.

```sql
CREATE TRIGGER E2_KEY
BEFORE INSERT ON E2
REFERENCING NEW AS N
FOR EACH ROW
WHEN (EXISTS (SELECT * FROM E2 WHERE (N.B1, N.B2) = (E2.B1, E2.B2)))
SIGNAL SQLSTATE '70001' ('La coppia (B1, B2) non può essere duplicata!');
```
