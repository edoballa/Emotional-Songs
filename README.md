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
ATTENZIONE: Per motivi di build della jar i file eseguibili non si trovano nella cartella bin, ma sono nelle cartelle compresse dei rispettivi progetti.

## Requisiti Tecnici

- **Linguaggio**: Java (versione 8 o successiva)
- **Piattaforme Supportate**: Windows, macOS, Linux

## Istruzioni per l'Esecuzione

**DB INIT**
Assicurarsi che il database postgres sia acceso e che, però, non ci sia nessun utente collegato al database con nome "dbes".
- Scompattare la cartella compressa e accedere alla cartella Lab-B-Server all’interno della cartella DbInit
- Aprire il command prompt e lanciare il comando cd {path}/DbInit/Lab-B-Server sostituendo a {path} il path corretto, nel mio caso : cd C:\Users\Edoardo\OneDrive\University\Laboratorio_B\Lab-B-Server
- Lanciare il comando java –jar shadeEmotionalSongs.jar per avviare il db-init
**Attenzione:** la finestra del command prompt NON va chiusa
**Attenzione:** se quando si avvia l’applicazione con il comando viene loggata un’eccezione del genere potrebbe significare che c’è un utente che sta usando il database dbes, è necessario scollegare l’utente per configurare il database. Inoltre è necessario chiudere e riavviare l’applicazione. Per maggiori dettagli consulta la documentazione.

**SERVER**
- Scompattare la cartella compressa e accedere alla cartella Server-Lab-B
- Aprire il command prompt e lanciare il comando cd {path}/Server-Lab-B sostituendo a {path} il path corretto, nel mio caso : cd C:\Users\Edoardo\OneDrive\University\Laboratorio_B\Server-Lab-B
- Lanciare il comando java -jar shadeEmotionalSongs.jar per avviare il server
**Attenzione:** la finestra del command prompt NON va chiusa.

**CLIENT**
Il client non partirà se il server non è acceso.
- Scompattare la cartella compressa e accedere alla cartella Lab.B all’interno della cartella Client
- Aprire il command prompt e lanciare il comando cd {path}/Client/Lab.B sostituendo a {path} il path corretto, nel mio caso: cd C:\Users\Edoardo\Desktop\University\Laboratorio_B\Lab.B
- Lanciare il comando java –jar shadeEmotionalSongs.jar per avviare il client
**Attenzione:** la finestra del command prompt NON va chiusa.
**Attenzione:** se quando si avvia l’applicazione con il comando viene loggata un’eccezione del genere potrebbe significare che il server non è acceso. Per maggiori dettagli consulta la documentazione.
