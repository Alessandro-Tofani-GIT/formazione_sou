# Progetto DevOps Everywhere con Vagrant e Apache

## Descrizione

Questo progetto utilizza **Vagrant** per creare una macchina virtuale Ubuntu 22.04 (Jammy Jellyfish) configurata come un server web Apache. All'avvio, il provisioning esegue l'installazione di Apache e crea una pagina HTML personalizzata.

---

## Dettagli della configurazione

- **Box Vagrant:** `ubuntu/jammy64` (Ubuntu 22.04 LTS)
- **Rete:** rete privata con IP `192.168.33.10`
- **Software installato:** Apache2
- **Pagina web:** un file HTML personalizzato in `/var/www/html/index.html`

---

## Funzionamento del provisioning

Durante la fase di provisioning, il sistema esegue automaticamente:

1. Aggiornamento della lista dei pacchetti (`apt-get update`).
2. Installazione del server web Apache (`apt-get install -y apache2`).
3. Scrittura di una pagina HTML personalizzata, completa di struttura, stile e contenuti testuali.
4. Riavvio del servizio Apache per applicare le modifiche e rendere visibile la pagina.

---

## Come usare il progetto

1. Clona il repository contenente il Vagrantfile.
2. Assicurati di avere installato Vagrant e VirtualBox.
3. Avvia la macchina virtuale con:
   vagrant up

---

## Requisiti

- [Vagrant](https://www.vagrantup.com/downloads)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) 
