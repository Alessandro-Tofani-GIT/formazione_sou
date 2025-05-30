# Esercizi Academy DevOps Track 1
---
## Benvenuto in formazione_sou

In questo repository sono stati pubblicati gli esercizi svolti durante il percorso formativo presso l'Academy di Sourcesense. I contenuti presenti all'interno delle cartelle indicate fanno riferimento agli esercizi proposti nella Track 1.

---

### Ping_pong

All'interno della directory ping_pong è presente un esercizio che simula un comportamento "ping-pong" tra due container. Il meccanismo prevede che, in ogni momento, solo uno dei due container sia attivo mentre l'altro resta inattivo. L'alternanza tra i due avviene automaticamente grazie a un cron job, che verifica l'orario ogni minuto.
Nei minuti pari, il primo container viene avviato (se non è già attivo) e il secondo viene fermato.
Nei minuti dispari, accade il contrario: il primo container viene fermato e il secondo avviato.

---

### Step8

Nella directory Step8 sono stati aggiunti file README.md contenenti commenti tecnici volti a descrivere il funzionamento di ciascuno script. Questa documentazione esterna è finalizzata a migliorare la comprensione del codice.

---

### Devops_everywhere

All'interno della directory Devops_everywhere è presente un Vagrantfile che automatizza la creazione e configurazione di una macchina virtuale basata su Ubuntu. Questo file Vagrant esegue una serie di operazioni per preparare un ambiente web funzionante:

- Crea una macchina virtuale Ubuntu utilizzando Vagrant.
- Configura una rete privata, rendendo la VM accessibile localmente tramite un indirizzo IP specifico.
- Installa Apache, il server web open-source, se non è già presente.
- Genera una pagina HTML che contiene il testo "Devops_Everywhere" come contenuto visibile.
- Riavvia il servizio Apache per applicare tutte le modifiche e rendere la pagina accessibile tramite il browser.


