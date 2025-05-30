# Pulizia dei File di Log

## Descrizione

Questo script ha lo scopo di pulire i file di log presenti nella directory `/var/log` del sistema. In particolare, l'operazione si concentra sui seguenti file:

- **messages**: File di log contenente messaggi generali di sistema.
- **wtmp**: File di log che tiene traccia degli accessi e dei logout degli utenti al sistema.

Lo script svuota il contenuto di entrambi i file, liberando spazio su disco e contribuendo alla gestione dei file di log nel sistema.

## Funzionamento dello Script

Lo script esegue le seguenti operazioni:

1. **Accesso alla directory `/var/log`**: Lo script si sposta nella directory che contiene i file di log.
   
2. **Pulizia dei file di log**:
   - Viene utilizzato il comando `cat /dev/null > messages` per svuotare il contenuto del file di log `messages`.
   - Viene utilizzato il comando `cat /dev/null > wtmp` per svuotare il contenuto del file di log `wtmp`.

## Esecuzione dello Script

Per eseguire lo script, utilizzare i seguenti comandi:

1. **Accedere alla directory contenente lo script**:
   
   ```bash
   cd /percorso/del/script


