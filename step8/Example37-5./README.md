# Un semplice database di indirizzi

## Descrizione

Questo script utilizza un array associativo per memorizzare gli indirizzi di tre persone. In particolare, i nomi (Charles, John, Wilma) sono le chiavi, mentre gli indirizzi sono i valori associati. Dopo aver memorizzato i dati nell'array, lo script stampa l'indirizzo di ogni persona.

Alla fine dello script, viene utilizzato il comando `echo ${!address[*]}` per stampare una lista di tutte le chiavi nell'array, ovvero i nomi delle persone.

## Funzionamento dello Script

1. **Creazione dell'array associativo**: 
   Lo script crea un array associativo in cui le chiavi sono i nomi (Charles, John, Wilma) e i valori sono gli indirizzi corrispondenti.

2. **Stampa degli indirizzi**: 
   Una volta che i dati sono stati memorizzati, lo script stampa l'indirizzo di ciascuna persona.

3. **Stampa delle chiavi**: 
   Alla fine dello script, con il comando `echo ${!address[*]}`, vengono visualizzati tutti i nomi (le chiavi dell'array).

## Requisiti

Lo script richiede un ambiente di shell che supporti gli array associativi, come **Bash**.

## Esecuzione dello Script

Per eseguire lo script, basta lanciare il comando:

```bash
./address_database.sh

