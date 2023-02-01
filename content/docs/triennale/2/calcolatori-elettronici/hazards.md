# Hazards

## Problema

Abbiamo delle istruzioni che provocano **hazards**.

## Alee strutturali

> ⚠️ Risorsa condivisa tra più stadi (es. memoria).

### Come si risolve?

- Duplicazione della risorsa. Lo facciamo per esempio per l’ALU, che dovrebbe essere condivisa tra la fase di EXECUTE e quella di FETCH. Non sempre va bene ovviamente.
- Serializzazione degli accessi.
- [ADVANCED] Caches ovunque e facciamo finta di aver duplicato la risorsa.

## Alee di Dato

> ⚠️ Un istruzione legge qualcosa che è stato modificato da un’altra istruzione che è ancora in pipeline (es. _Read After Write - ***RAW***, jump a registro appena modificato_)

### Come si risolve?

- Forwarding: colleghiamo all’EX le fasi più avanti in modo tale che l’u.c. possa scegliere se utilizzare i registri provenienti dalla fase di DECODE _(stale)_ oppure quelli appena creati _(forwarded)_.

  Risolve quasi tutte le RAW senza stallare la pipeline.

- Se l’istruzione che modifica (quella da cui la nostra istruzione attuale nell’EX dipende) è una LOAD è un problema. Perchè? Perchè c’è accesso in memoria. Che cazzo forwardi? nulla. Quindi bisogna aspettare la fine di MEM.

  In questo caso si può ricorrere alla _delayed load_ perchè se la nostra istruzione è nella fase di EX, la LOAD sarà in fase di WB, quindi possiamo prendere già il valore presente nel registro appena e **forwardarlo alla fase di EX**.

> 🔥 La _delayed load_ è fattibile solamente se ho il forward.

## Alee di Controllo

La `BRANCH` e la `JUMP`, oltre ad avere un problema di alea di dato se faccio jump/branch ad un registro appena modificato, hanno anche un **alea di controllo**.

In generale per entrambe possiamo ottimizzare l’archittetura per avere che il risultato della JUMP/BRANCH (nella EX) mi faccia caricare direttamente la prossima istruzione corretta.

Mentre per la JUMP, non posso fare nient’altro, per la branch posso provare a predirre se il jump sarà taken or not. Per fare questo ci sono vari modi.

La migliore (vista) è il BTB, perchè sbaglio molto meno di qualsiasi modo (sicuramente non ha senso l’_always stall_ e con la _predict not taken_ sbaglio molte più volte)
