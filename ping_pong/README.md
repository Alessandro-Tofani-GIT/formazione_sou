# Ping-Pong Docker Containers con Vagrant

## Descrizione

Questo progetto utilizza **Vagrant** per creare due macchine virtuali basate su Ubuntu 24.04. Ogni macchina è configurata per eseguire un container Docker che esegue l'immagine `ealen/echo-server`. L'attivazione dei container segue una logica "ping-pong":  
- Il **nodo 1** esegue il container nei minuti **pari**
- Il **nodo 2** lo esegue nei minuti **dispari**

La gestione dell'attivazione e disattivazione dei container è automatizzata tramite **cron job** su ciascuna macchina.

## Struttura dei nodi

### Nodo 1 (`node1`)
- **Hostname**: `master.local`
- **IP Privato**: `192.168.3.20`
- **Ruolo**: Avvia il container Docker nei minuti **pari**
- **Servizi installati**: `docker.io`
- **Cron job**: Esegue lo script `/usr/local/bin/docker_start_stop.sh` ogni **2 minuti** a partire dal minuto 0

### Nodo 2 (`node2`)
- **Hostname**: `master2.local`
- **IP Privato**: `192.168.3.21`
- **Ruolo**: Avvia il container Docker nei minuti **dispari**
- **Servizi installati**: `docker.io`
- **Cron job**: Esegue lo script `/usr/local/bin/docker_start_stop.sh` ogni **2 minuti** a partire dal minuto 1

## Funzionamento dello script `docker_start_stop.sh`

Lo script esegue le seguenti operazioni:
1. **Controlla** se il container chiamato `echo-server` è già presente.
2. Se il container **non esiste**, lo avvia con l'immagine `ealen/echo-server`.
3. Se il container **esiste ma è spento**, lo avvia.
4. Dopo **60 secondi**, lo **spegne**.

Lo script viene aggiunto a `/usr/local/bin/` e reso eseguibile.

## Requisiti

- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/)













