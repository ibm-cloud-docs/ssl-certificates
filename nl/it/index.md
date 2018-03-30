---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introduzione ai certificati SSL  


## Prima di cominciare

L'introduzione a SSL richiede un pò di pianificazionie. Completa i seguenti prerequisiti.

1. Decidi dove ottenere il certificato
2. Informati sui tipi di certificati, la lunghezza della chiave e la durata
3. Scegli un nome comune
4. Informati sulle regole socket
5. Genera il CSR

Per ulteriori informazioni, vedi [Pianificazione per i certificati SSL](planning-ahead-ssl.html).

## Ordine dei certificati SSL

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Seleziona **Security > Certificati SSL >** per accedere alla schermata dei certificati SSL.
3. Devi selezionare il tipo e la durata del certificato, inviare il testo del CSR, immettere alcuni dettagli aggiuntivi e poi confermare il pagamento.

## Installazione e verifica
Dopo che i processi di ordinazione e verifica vengono completati, riceverai un'email dall'autorità di certificazione che include il tuo certificato così come ogni certificato intermedio necessario. Il metodo per l'installazione dipende dal software che stai utilizzando ma il risultato dovrebbe essere lo stesso. Una volta completato, dovresti essere in grado di andare in <http://host.yourdomain.com> e vedere il tuo contenuto mentre vedi anche il lucchetto SSL che i browser utilizzano per indicare una sesscione crittografata. Se ottieni un avviso, allora esistono passi che devi eseguire.

## Passi successivi

Dopo che la verifica viene eseguita con successo, puoi accedere alla schermata dei certificati SSL, per [aggiornare](view-and-update-ssl-certificate.html), [scaricare](download-ssl-certificate-details.html), [eliminare](delete-ssl-certificate.html), o [importare](import-ssl-certificate.html) certificati SSL esistenti nello strumento.
