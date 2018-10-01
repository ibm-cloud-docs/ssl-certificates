---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Pianificazione di SSL

L'introduzione a SSL richiede un po' di pianificazione. Completa i seguenti prerequisiti.

1. Decidi dove ottenere il certificato
2. Informati sui tipi di certificati, la lunghezza della chiave e la durata
3. Scegli un nome comune
4. Informati sulle regole socket
5. Genera il CSR

## Decidi dove ottenere il certificato

I certificati SSL possono essere ottenuti internamente alla tua organizzazione o dall'autorità di certificazione (CA) come Verisign, RapidSSL, Thawte e altri.  

Per un piccolo gruppo in una architettura controllata, come degli impiegati che utilizzano un sito intranet, puoi acquisire un certificato autofirmato che ogni impiegato installa nel suo browser. Puoi anche impostare da solo un'autorità di certificazione (CA) locale per generare i certificati da usare nella tua organizzazione.

Per un gruppo più grande e diverso, l'utilizzo di un certificato SSL da un'origine standard permette l'accesso senza una configurazione specializzata. I web browser moderni sono configurati per assicurare certificati SSL emessi dalle autorità di certificazione (CA).

## Informati sui tipi di certificati, la lunghezza della chiave e la durata

Dopo aver deciso dove ottenere il tuo certificato, riesamina le seguenti opzioni dei tipi di certificati e le loro corrispondenti disponibilità, lunghezza della chiave e durata.

|              Tipi di certificati          |  Disponibilità                     |  Lunghezza chiave                |  Durata                  |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Convalida dominio (DV)                   | Disponibile velocemente                 | 1024 bit o 2048 bit       | 1 o 2 anni             |
|Convalida organizzazione (OV)             | 2-3 giorni o fino a una settimana          | 1024 bit o 2048 bit       | 1 o 2 anni             |
|Convalida estesa (EV)                 | 2-3 giorni o fino a una settimana          | solo 2048 bit              | 1 o 2 anni             |
{: caption="Tabella 1. Tipi di certificati" caption-side="top"}   


## Scegli un nome comune

Il nome comune utilizzato nel certificato è il nome host per il sito web. Il nome host e il nome comune del certificato devono corrispondere altrimenti i browser emettono un'avvertenza. Se il tuo sito è web1.mydomain.com, utilizzalo come nome comune. Se utilizzi anche images.mydomain.com, hai bisogno o di un certificato jolly (che è disponibile in {{site.data.keyword.cloud}}) o di impostare più certificati. Se scegli un nome comune sbagliato, ci sono passi che possono essere intrapresi per sistemare un ordine di certificato o per revocare e immettere nuovamente il nome comune corretto.  

## Informati sulle regole socket

I certificati SSL sono limitati a un certificato per socket. Un socket è un indirizzo IP e una combinazione di porta, come 1.2.3.4:443 (1.2.3.4:444 è un socket diverso). Per le applicazioni come SMTP/POP3 o FTP, la regola del socket non ha importanza. Tuttavia conta per l'HTTP a causa del suo coinvolgimento con l'hosting virtuale.

L'host virtuale è il metodo per cui puoi ospitare 20, 30, 100 siti web in un indirizzo IP. L'hosting virtuale funziona perché i browser moderni superano un campo chiamato il lettore host come parte delle loro richieste. Questo campo assomiglia a “Host: web1.mydomain.com” e indica il server web del sito al quale stai cercando di accedere. Nel caso di HTTPS (HTTP over SSL), il server web deve selezionare il certificato SSL da inviare al client prima di vedere l'intestazione dell'host, che è il motivo per cui un socket può avere solo un certificato.

Puoi assegnare ogni sito web abilitato SSL al proprio socket variando l'indirizzo IP o la porta. Tieni a mente che se modifichi la porta da 443/tcp, gli utenti devono includere il numero di porta nel loro URL, come https://web1.mydomain.com:444.

## Genera il CSR

Puoi generare il CSR (Certificate Signing Request) utilizzando il software sul server web. Per i sistemi UNIX, utilizza il pacchetto OpenSSL. Per Windows c'è una procedura guidata che è accessibile dalla scheda Directory Security delle proprietà del sito web nel gestore IIS. Se stai utilizzano un pannello di controllo, fai riferimento alle specifiche informazioni per quel pannello di controllo.

Durante la generazione del CSR, crei una chiave privata. Non perdere, cancellare o condividere la chiave privata. È da mantenere privata sul server web. Alcuni programmi di utilità per la generazione del CSR ti forniscono anche la capacità di creare una passphrase per la chiave privata. Non farlo a meno che non prevedi di accedere al server ogni volta che il software del server web viene riavviato. In aggiunga, non applicare una challenge phrase al CSR.

