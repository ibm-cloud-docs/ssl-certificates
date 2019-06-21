---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestione dei certificati SSL
{: #managing-ssl-certificates}

Puoi gestire i tuoi certificati SSL nella console {{site.data.keyword.cloud}}. Non solo questo può servire come un repository per la gestione dei tuoi certificati, ma è anche necessario quando si utilizzano i servizi che possono utilizzare o richiedere certificati.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza**, seleziona **SSL > Certificati > Gestisci Certificati**.


Si presenta un elenco dei tuoi certificati correnti insieme alle informazioni riguardanti lo stato.

Puoi cercare, scaricare parti di un certificato o una versione formattata PEM, oppure riesaminare la scadenza dei tuoi certificati. Puoi anche visualizzare quanti servizi stanno attualmente utilizzando ogni certificato. Questo ti consente di sapere se l'azione deve essere eseguita quando un certificato sta raggiungendo la scadenza.

## Aggiunta di un certificato

Quando sei pronto ad aggiungere un certificato, seleziona **Aggiungi certificato** nel menu di navigazione secondario o nel titolo dell'elenco del certificato. Ti viene solo richiesto di fornire il certificato e la sua chiave privata. Tuttavia, non fornendo un certificato intermedio quando il tuo emittente ne fornisce uno, può causare una catena di certificati rotta e una convalida impropria per gli utenti o i servizi associati.

Le chiavi private che richiedono una passphrase non possono essere memorizzate.
{:note}

Una volta aggiunti, i seguenti campi sono derivati direttamente dai tuoi certificati:

* Nome comune
* Nome organizzazione
* Periodo di validità 

## Modifica di un certificato

Attivando il triangolo a sinistra di un certificato si rivelano le parti del certificato nella loro interezza. Ciò permette anche di modificare le parti del certificato. Una nota può essere aggiunta e, quando necessario, il certificato può essere rimosso. Viene anche elencata una lista di servizi che stanno attualmente utilizzando il certificato.

Solo i certificati che non sono associati ai servizi possono avere la loro chiave privata, il certificato o le parti del certificato intermedio aggiornati.  Il certificato inoltre non può essere rimosso. Puoi modificare la nota in qualsiasi momento.

## Rimozione di un certificato

Per rimuovere un certificato, segui i passi per modificarlo, seleziona "Conferma rimozione certificato" e salva.

## Utilizzo dell'API

Per un esempio di modifica dei certificati utilizzando l'API, consulta [Gestione SSL ![Icona collegamento esterno](../../icons/launch-glyph.svg "Icona collegamento esterno")](http://sldn.softlayer.com/article/ssl-management){: new_window}.
