# Verifica se sei Root o No in Bash

## Descrizione

Questo script in **Bash** è progettato per verificare se l'utente che esegue lo script ha privilegi da **root**. Lo script esegue questa verifica in due modi:
1. Controlla l'UID dell'utente.
2. Confronta il nome dell'utente con "root".

Se l'utente ha privilegi da root (UID 0 o nome utente "root"), lo script stamperà un messaggio che conferma che l'utente è root. Altrimenti, verrà stampato un messaggio che afferma che l'utente è un "utente ordinario".

## Funzionamento dello Script

1. **Verifica tramite UID**:
   Il primo controllo confronta l'UID dell'utente con `0`, che è l'UID riservato per l'utente root. Se il confronto è vero, significa che l'utente è root.

2. **Verifica tramite nome utente**:
   Il secondo controllo verifica se il nome dell'utente corrente è "root" utilizzando il comando `id -nu` o `whoami`. Se il nome dell'utente è root, viene confermato che l'utente è root.

## Conclusioni

Questo script è un esempio di come verificare se un utente ha privilegi da root in Bash
