# Emotional Songs

## Project Overview

Emotional Songs è un progetto sviluppato nell'ambito del Laboratorio Interdisciplinare A e B presso l'Università degli Studi dell'Insubria. L'obiettivo dell'applicazione è permettere agli utenti di creare playlist musicali e annotare le emozioni suscitate da ciascun brano, offrendo una panoramica aggregata delle emozioni provate durante l'ascolto di diverse canzoni.

## Funzionalità

- **Consultazione del repository di canzoni**: Gli utenti possono cercare brani per titolo, autore o anno senza necessità di registrazione.
- **Registrazione e autenticazione**: Gli utenti possono registrarsi e accedere al sistema per creare playlist personalizzate.
- **Creazione di playlist**: Gli utenti registrati possono creare una o più playlist con i brani disponibili nel repository.
- **Inserimento delle emozioni**: Gli utenti possono aggiungere le emozioni provate durante l'ascolto delle canzoni, utilizzando una scala di intensità da 1 (per niente) a 5 (molto).
- **Visualizzazione emozioni aggregate**: Per ogni brano è possibile visualizzare in modo aggregato le emozioni inserite da tutti gli utenti.

## Emozioni Supportate

L'applicazione consente di annotare le seguenti emozioni:

- **Amazement**: Meraviglia o felicità
- **Solemnity**: Transcendenza, ispirazione, brividi
- **Tenderness**: Sensualità, affetto, amore
- **Nostalgia**: Sentimenti malinconici o sentimentali
- **Calmness**: Rilassamento, serenità
- **Power**: Forza, eroismo, energia
- **Joy**: Allegria, voglia di ballare
- **Tension**: Nervosismo, impazienza
- **Sadness**: Tristezza, malinconia

## File Utilizzati

L'applicazione utilizza diversi file di dati per memorizzare le informazioni:

- `Canzoni.dati`: File contenente le informazioni sui brani musicali (titolo, autore, anno, ecc.).
- `UtentiRegistrati.dati`: File contenente i dati degli utenti registrati.
- `Playlist.dati`: File che memorizza le playlist create dagli utenti.
- `Emozioni.dati`: File che conserva le emozioni associate a ciascun brano.

## Struttura del Progetto

- `src/`: Contiene il codice sorgente Java.
- `bin/`: Contiene il codice compilato.
- `data/`: Contiene i file di dati (canzoni, utenti, playlist, emozioni).
- `doc/`: Contiene la documentazione (manuale utente e tecnico).

## Requisiti Tecnici

- **Linguaggio**: Java (versione 8 o successiva)
- **Piattaforme Supportate**: Windows, macOS, Linux
