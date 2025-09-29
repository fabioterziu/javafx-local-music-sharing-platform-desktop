# 🎵 PIATTAFORMA LOCALE DI CONDIVISIONE MUSICALE DESKTOP JAVAFX

## BREVE DESCRIZIONE:
Elaborato sviluppato in coppia per l'esame di Ingegneria del Software [Anno 2025].  

L'applicazione permette la gestione collaborativa di materiale musicale (testi/audio/video/youtube).  
- Soltanto gli utenti autorizzati da un profilo admin potranno accedere.  
- Gli utenti possono avere la possibilità di caricare/scaricare materiale musicale, commentare e annotare brani.

(Le password vengono hashate con SHA-256 prima di essere memorizzate nel database)


## TECNOLOGIE UTILIZZATE
- linguaggio: JAVA
- framework GUI: JAVAFX
- markup UI: FXML
- stile UI: CSS
- database: SQLITE

## PATTERN
- Architetturale: MVC
- Design: DAO, SINGLETON, SINGLETON (lazy)
  
## DOCUMENTAZIONE E TESTING  
(diagrammi e test sono focalizzati sulle funzionalità più critiche)  

- Use Case e schede di specifica
- Sequence diagram di dettaglio per i principali Use Case
- Activity Diagram relativo alle modalità di interazione/operatività del software
- Class Diagram e Sequence diagram del software progettato
    
- Test degli sviluppatori
- Unit test
- Integration test sulle funzionalità più critiche
- Test degli utenti generici



## NOTE

**(Per un'illustrazione più dettagliata consultare [“Relazione.pdf”](Relazione.pdf))**

- **stato del progetto:**
  Il progetto è concluso e funzionante.  
  È prevista però una fase di refactoring volta a migliorare ulteriormente la separazione delle responsabilità.  
  Nello specifico si procederà alla suddivisione della logica di business dai controller in apposite classi di servizio, come è stato già fatto per 'TrackController' e 'TrackService'

- Credenziali admin:  
  username: admin  
  password: admin

- Gestione chiave YOUTUBE API:
  per questioni di sicurezza, la chiave è gestita esternamente.  
  Prima di avviare l'applicazione è necessario impostare la variabile "YOUTUBE_API_KEY" da terminale:  
  per linux/macos:  
  export YOUTUBE_API_KEY="inserire_la_chiave"  
  altrimenti:  
  l'applicazione viene eseguita comunque, ma senza la possibilità di visionare video youtube all'interno dell'app
