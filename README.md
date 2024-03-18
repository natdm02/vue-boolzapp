VUE-BOOLZAPP
===
- Milestone 1
Replica della grafica con la possibilità di avere messaggi scritti dall’utente (verdi) e dall’interlocutore (bianco) assegnando due classi CSS diverse
Visualizzazione dinamica della lista contatti: tramite la direttiva v-for, visualizzare nome e immagine di ogni contatto
- Milestone 2
Visualizzazione dinamica dei messaggi: tramite la direttiva v-for, visualizzare tutti i messaggi relativi al contatto attivo all’interno del pannello della conversazione
Click sul contatto mostra la conversazione del contatto cliccato
- Milestone 3
Aggiunta di un messaggio: l’utente scrive un testo nella parte bassa e digitando “enter” il testo viene aggiunto al thread sopra, come messaggio verde
Risposta dall’interlocutore: ad ogni inserimento di un messaggio, l’utente riceverà un “ok” come risposta, che apparirà dopo 1 secondo.
- Milestone 4
Ricerca utenti: scrivendo qualcosa nell’input a sinistra, vengono visualizzati solo i contatti il cui nome contiene le lettere inserite (es, Marco, Matteo Martina -> Scrivo “mar” rimangono solo Marco e Martina)
- Milestone 5 - opzionale
Cancella messaggio: cliccando sul messaggio appare un menu a tendina che permette di cancellare il messaggio selezionato
Visualizzazione ora e ultimo messaggio inviato/ricevuto nella lista dei contatti 

## SVOLGIMENTO:

1. Destrutturazione vue.
2. Array di contatti.(Ogni contatto ha un nome, una img, uno stato di visibilità e un array di messaggi. Ogni messaggio ha una data, un testo e uno stato.)
3. Oggetto datetime dalla libreria Luxon per gestire le date e gli orari. 
4. Dati dell'applicazione Vue: Nell'oggetto data, vengono definiti i dati utilizzati nell'applicazione.
5. Metodi: 
- chat(i): Cambia l'indice del contatto al clic su un contatto.
- sendMessage(): Invia un messaggio aggiungendo un nuovo oggetto all'array dei messaggi del contatto e avvia una risposta dopo un secondo.
- answer(): Aggiunge una risposta automatica dopo un secondo dall'invio del messaggio.
- search(): Filtra i contatti in base al testo di ricerca inserito dall'utente.
- deleteMsg(i): Cancella un messaggio dall'array dei messaggi del contatto attivo.
- formatDate(myDate): Formatta la data dei messaggi mostrando solo l'orario.

