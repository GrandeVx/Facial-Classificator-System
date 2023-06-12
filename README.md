## Obiettivi
Il presente codice implementa una soluzione avanzata per la gestione di immagini con volti utilizzando gli algoritmi di clustering e embedding. 

Gli obiettivi principali del codice sono i seguenti:

  1. Acquisire un database di immagini senza etichette e generare un dataset apposito.
  2. Applicare algoritmi di clustering per creare raggruppamenti di immagini.
  3. Salvare tutte le informazioni rilevanti per ogni immagine con volto noto.
  4. Generare gli embedding medi per ogni cluster.
  5. Analizzare una nuova immagine e determinare se fa parte di un cluster esistente.

## Progressi

I progressi finora compiuti includono:

 - Caricamento del modello FaceNet512.
 - Preparazione delle immagini, inclusa la conversione dei formati HEIC in JPG.
 - Generazione del dataset a partire dalle immagini presenti nel database.
 - Identificazione e embedding di singoli volti presenti nel database.
 - Generazione dei cluster utilizzando l'algoritmo DBSCAN.
 - Calcolo del valore ottimale del parametro eps per DBSCAN.
 - Salvataggio dei cluster e dell'intero database.
 - Calcolo degli embedding medi per ogni cluster.
 - Implementazione del sistema per l'acquisizione di nuove immagini.
 - Utilizzo di un modello NearestNeighbors per la ricerca del volto più vicino.

## Uso del codice
Per utilizzare il codice, è necessario eseguire le seguenti operazioni:

 1. Clonare il repository DeepFace con il comando: git clone https://github.com/serengil/deepface.git.
 2. Installare le dipendenze necessarie.
 3. Eseguire il codice fornito nel file main.ipynb.

 > Si prega di notare che è necessario disporre di un dataset di immagini senza etichette all'interno della cartella "data" prima di eseguire il codice.