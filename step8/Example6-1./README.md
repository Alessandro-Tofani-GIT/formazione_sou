# Gestione dello Status di Uscita in Bash

## Descrizione

Questo script in **Bash** mostra come gestire e interpretare lo status di uscita (exit status) dei comandi. Ogni comando eseguito in Bash restituisce un codice di uscita che indica se l'esecuzione è avvenuta correttamente o meno.

Lo script esegue i seguenti passi:
1. Esegue un comando valido e stampa il suo exit status.
2. Esegue un comando non valido e stampa il suo exit status.
3. Esce dallo script con un codice di uscita personalizzato.

## Funzionamento dello Script

1. **Esecuzione di un comando valido**: 
   Lo script esegue il comando `echo hello` e stampa il suo exit status usando `$?`. Poiché `echo` è un comando valido, il codice di uscita sarà `0`, che indica il successo.

2. **Esecuzione di un comando non valido**:
   Viene eseguito un comando non valido (`lskdf`), che restituirà un codice di uscita diverso da `0`. In questo caso, l'exit status sarà diverso da zero, indicando che il comando non è riuscito.

3. **Codice di uscita personalizzato**:
   Lo script termina con un codice di uscita personalizzato `113`. Questo codice verrà restituito quando lo script terminerà, e può essere verificato eseguendo `echo $?` dopo la terminazione dello script.

## Conclusioni

Questo script è un esempio di come gestire lo status di uscita in Bash. L'uso dell'exit status è fondamentale per determinare se i comandi sono stati eseguiti correttamente o se si sono verificati errori durante l'esecuzione di uno script.
