# Ping pong di un docker container tra  due nodi

## 🇬Description

The Vagrantfile automatically generates two Ubuntu 24.04 virtual machines with Docker preinstalled. On each machine, a script named docker_start_stop.sh is created, which starts a container called echo-server, keeps it running for 60 seconds, and then stops it. The script is executed automatically via cron: on even minutes on node1, and on odd minutes on node2. This allows the container to run alternately between the two virtual machines. In this way, the container is started alternately on each machine. The resulting environment is useful for simulations, basic orchestration tests, or failover scenarios.


## 🇮Descrizione

Il Vagrantfile genera due macchine virtuali Ubuntu 24.04 con Docker preinstallato. Su ciascuna viene creato uno script chiamato docker_start_stop.sh che avvia un container chiamato echo-server, lo mantiene attivo per 60 secondi e poi lo arresta. Lo script è eseguito automaticamente tramite cron: nei minuti pari su node1, nei minuti dispari su node2. Questo permette un'esecuzione alternata del container tra le due VM.In questo modo, il container viene avviato alternativamente sulle due macchine. L’ambiente risultante è utile per simulazioni, test di orchestrazione base o scenari di failover.


