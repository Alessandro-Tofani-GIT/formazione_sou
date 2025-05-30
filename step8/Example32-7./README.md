# Implementazione Semplice di una Barra di Progresso

## Descrizione

Questo script ha l'obiettivo principale di mostrare una **barra di progresso**.
Il funzionamento è il seguente:
- Avvia un processo in background che stampa un punto (`.`) ogni secondo, utilizzando un ciclo infinito (`while true`).
- Quando si preme `^C` (Ctrl+C), viene attivato il seguente comando tramite `trap`:

```bash
trap "echo !; kill -USR1 $pid; wait $pid" EXIT
```

### Cosa fa questo comando?

1. Stampa un punto esclamativo (`!`).
2. Invia un segnale `SIGUSR1` al processo identificato da `$pid`.
3. Attende la terminazione del processo con `wait $pid`.

Nel processo secondario, è presente un `trap` configurato per ricevere `SIGUSR1` e, al ricevimento del segnale, eseguire il comando `exit`, che interrompe il ciclo infinito.

### Nota Importante

Se si commenta il comando `trap` nel processo principale, il loop non verrà più interrotto con `^C`. Questo accade perché il segnale `SIGUSR1` non viene più inviato, rendendo necessario l'intervento manuale tramite il comando `kill`.

## Esempio di utilizzo

```bash
#!/bin/bash







