#############################################################################################################
Per motivi di build della jar i file eseguibili non si trovano nella cartella bin, 
ma sono nelle cartelle compresse dei rispettivi progetti.
In questo file README verranno elencati i passaggi base per l'avvio delle applicazioni.
Eventuali errori o maggiori dettagli su come configurare e far funzionare al meglio l'applicazione sono 
contenuti all'interno del documento tecnico e del manuale utente.
Nel dettaglio:
- Capitolo 11 -> Configurazione DbInit (Doc Tecnico)
- Capitolo 12 -> Configurazione Server (Doc Tecnico)
- Capitolo 3 -> Predisposizione ambiente e avvio del programma (Manuale Utente)

#############################################################################################################
		ISTRUZIONI BASE PER LANCIARE GLI ESEGUIBILI DI DBINIT, SERVER E CLIENT
#############################################################################################################
						DB INIT
Assicurarsi che il database postgres sia acceso e che, però, non ci sia nessun utente collegato al database 
con nome “dbes”.
# Scompattare la cartella compressa e accedere alla cartella Lab-B-Server all’interno della cartella DbInit. 
# Aprire il command prompt e lanciare il comando cd {path}/DbInit/Lab-B-Server sostituendo a {path} il path 
  corretto, nel mio caso : cd C:\Users\Diana\OneDrive\University\Laboratorio_B\Lab-B-Server 
# Lanciare il comando java –jar shadeEmotionalSongs.jar per avviare il db-init.

!# Attenzione: la finestra del command prompt NON va chiusa
!# Attenzione: se quando si avvia l’applicazione con il comando viene loggata un’eccezione del genere
   potrebbe significare che c’è un utente che sta usando il database dbes, è necessario scollegare
   l’utente per configurare il database. Inoltre è necessario chiudere e riavviare l’applicazione.
   Per maggiori dettagli consulta la documentazione.

						SERVER
# Scompattare la cartella compressa e accedere alla cartella Server-Lab-B.
# Aprire il command prompt e lanciare il comando cd {path}/Server-Lab-B sostituendo a {path} il path corretto, 
  nel mio caso : cd C:\Users\Diana\OneDrive\University\Laboratorio_B\Server-Lab-B
# Lanciare il comando java -jar shadeEmotionalSongs.jar per avviare il server.

!# Attenzione: la finestra del command prompt NON va chiusa.

						CLIENT
Il client non partirà se il server non è acceso.
# Scompattare la cartella compressa e accedere alla cartella Lab.B all’interno della cartella Client. 
# Aprire il command prompt e lanciare il comando cd {path}/Client/Lab.B sostituendo a {path} il path corretto,
  nel mio caso: cd C:\Users\Diana\Desktop\University\Laboratorio_B\Lab.B
# Lanciare il comando java –jar shadeEmotionalSongs.jar per avviare il client.

!# Attenzione: la finestra del command prompt NON va chiusa
!# Attenzione: se quando si avvia l’applicazione con il comando viene loggata un’eccezione del genere
   potrebbe significare che il server non è acceso. Per maggiori dettagli consulta la documentazione.
#############################################################################################################