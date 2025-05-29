# Esercizi Academy DevOps Track 1
---
## Benvenuto in formazione_sou

In questo repository ho pubblicato gli esercizi presenti in Track 1 su cui ho lavorato.

---

### Ping_pong

All'interno della directory ping_pong è presente un esercizio che simula un comportamento "ping-pong" tra due container. Il meccanismo prevede che, in ogni momento, solo uno dei due container sia attivo mentre l'altro resta inattivo. L'alternanza tra i due avviene automaticamente grazie a un cron job, che verifica l'orario ogni minuto.
Nei minuti pari, il primo container viene avviato (se non è già attivo) e il secondo viene fermato.
Nei minuti dispari, accade il contrario: il primo container viene fermato e il secondo avviato.

---

### Step8

Nella directory `Step8`, ho aggiunto dei commenti che spiegano il funzionamento di ciascuno script.

---

### Devops_everywhere

All'interno della directory Devops_everywhere è presente un Vagrantfile che automatizza la creazione e configurazione di una macchina virtuale basata su Ubuntu. Questo file Vagrant esegue una serie di operazioni per preparare un ambiente web funzionante:

- Crea una macchina virtuale Ubuntu utilizzando Vagrant.
- Configura una rete privata, rendendo la VM accessibile localmente tramite un indirizzo IP specifico.
- Installa Apache, il server web open-source, se non è già presente.
- Genera una pagina HTML che contiene il testo "Devops_Everywhere" come contenuto visibile.
- Riavvia il servizio Apache per applicare tutte le modifiche e rendere la pagina accessibile tramite il browser.


