---
title: Sistemi informativi e sistemi informatici
feed: show
date: 16-06-2022
---

Bisogna fare una distinzione:
- **dato**: valore misurato *(altezza)*
- **informazione**: si ottiene dall'elaborazione dei **dati** *(il più alto)*

Il **sistema informativo** è l'insieme di procedure che servono a *raccogliere dati* ed elaborarli per ricavarne *informazioni*, e ci sono 2 motivi per disporre di adeguate informazioni:
- **operativo**: per svolgere un'attività servono certe **informazioni**.
- **decisionale**: serve per programmare attività, controllare e valutare.

Il **sistema informatico** è un sottoinsieme del **sistema informativo** dedicato al trattamento *automatico* di **informazioni**, e la sua realizzazione si distingue in tre fasi.

| macrofase  | output  |
|---|---|
| raccolta richieste utenti | definizione requisiti |
| progettazione concettuale | modello della realtà  |
| realizzazione | insieme software d'implentazione  |

## Aspetti intensionale ed estensionale dei dati
I dati sono utili solo quando c'è una **semantica**, per cui serve descrivere cosa **rappresenta** un certo dato, e la **relazione** che lo lega agli altri:
- l'aspetto **estensionale** riguarda il valore effettivo del dato.
- l'aspetto **intensionale** riguarda l'interpretazione di un dato.

## File di dati e loro organizzazione
- **File o archivio dati**: insieme di dati correlati identificati da un nome *(indipendenti dal software di scrittura e lettura usato)*.
- **Registrazioni o record**: unità logiche di cui è fornito l'aspetto **intensionale** *(chiave e valore)*.
- **File system**: software di un **OS** che consente la gestione dei file.

Su un **file** si possono eseguire diverse operazioni:
- creazione
- apertura
- chiusura

Per quanto riguarda i **record**:
- inserimento
- modifica
- cancellazione
- ricerca

I **record** possono essere organizzati in vari modi:
- *sequenziale*, per cui bisogna scorrere tutti i record.
- *accesso diretto* (o casuale, random) tramite numero posizione.
- *indicizzato* tramite chiave.

## DBMS
È un software che gestisce grandi collezioni di dati **condivisi**, in modo **efficiente** ed **efficace** assicurando **affidabilità** e **sicurezza**, e alcune caratteristiche che lo differenziano dall'approccio del **file** system:
- **integrazione**: i dati sono strutturati in maniera integrata, senza ridondanze superflue, insieme all'aspetto **intensionale**, collegato ai **vincoli di integrità**.
- **indipendenza logica**: la logica applicativa è separata dalla struttura dei dati.
- **indipendenza fisica**: la struttura dei dati è separata dallo schema fisico dei file.
- **integrità**: il **DBMS** si occupa di verificare che i dati vengano aggiornati rispettando i vincoli definiti precedentemente.

Il **DBMS** mette a disposizione dei linguaggi per interagire con il database: 
- **DDL** *(Data Definition Language)*: serve a definire l'aspetto **intensionale** dei dati, i loro legami e i vincoli d'**integrità**.
- **DML** *(Data Manipulation Language)*: serve a gestire e utilizzare i dati, tramite *inserimento*, *eliminazione*, *aggiornamento*. A sua volta si divide in due categorie:
	- **ospitato**: linguaggi "immersi" in **linguaggi di programmazione**.
	- **autonomo**: indipendente, di tipo dichiarativo *(solitamente)*.

## Architettura logica di un DBMS
- **Livello fisico**: riguarda l'organizzazione dei dati e la memorizzazione.
- **Livello logico globale**: è la definizione dello **schema logico** sviluppata dal **DBA** *(DataBase Administrator)*.
- **Livello logico utente**: è lo spazio di lavoro personalizzato di ogni utente, definito dal **DBA** *(sono sottoinsiemi del modello logico, visibili da una "vista utente")*.

## Database e transazioni
I **DBMS** supportano accessi **concorrenti** da parte di più **utenti**, per cui bisogna risolvere tutta una serie di problematiche legate alla **concorrenza**, e alla generazioni di dati **incoerenti**.

La **transazione** è un'unità logica in cui il database viene trasformato, attraverso **una o più operazioni** *(se anche solo una non dovesse avere successo, va ripristinato lo stato iniziale)*. Di fatto, una **transazione** può avere diversi **stati** e **fasi**. %% TODO: elencali dopo, pag 1096 %%

Un **DBMS**, per essere tale, deve garantire le proprietà **ACID**:
- **Atomicity**: o si eseguono tutte le operazioni, o nessuna.
- **Consistency**: la transazione non deve violare i *vincoli d'integrità* del database.
- **Isolation**: le **transazioni** non devono essere dipendenti l'una dall'altra.
- **Durability**: una volta eseguita una **transazione**, il suo effetto è *permantente*.