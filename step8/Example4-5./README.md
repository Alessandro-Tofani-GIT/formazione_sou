# Gestione dei Parametri da Riga di Comando in Bash

## Descrizione

Questo script in **Bash** è progettato per gestire i parametri passati da riga di comando. Richiede almeno 10 parametri per essere eseguito correttamente. Lo script stampa il nome dello script stesso, i parametri passati e verifica se il numero minimo di parametri è stato fornito.

## Funzionamento dello Script

1. **Nome dello script**: Lo script stampa il nome del file eseguibile in due modi:
   - Con il comando `$0` per ottenere il nome completo del file.
   - Con il comando `basename $0`, che rimuove eventuali percorsi e lascia solo il nome del file.

2. **Verifica e Stampa dei Parametri**: Lo script verifica se i parametri specificati sono stati passati e li stampa uno alla volta. Per i parametri successivi al nono, è necessario utilizzare le parentesi graffe per accedere ai parametri (ad esempio, `${10}` per il decimo parametro).

3. **Verifica del Numero di Parametri**: Lo script verifica se il numero di parametri passati è inferiore al valore minimo richiesto (10 in questo caso). Se non vengono forniti abbastanza parametri, viene stampato un messaggio di errore.

## Conclusioni

Questo script è un buon esempio di come gestire i parametri da riga di comando in Bash. In particolare, mostra come gestire parametri numerici, come stampare il nome dello script e come garantire che venga passato un numero minimo di parametri per evitare errori.



