---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# FAQ: certificati SSL

## Perché il certificato SSL che ho ordinato non viene visualizzato automaticamente nella schermata dei certificati SSL?

I certificati SSL vengono emessi da un'autorità di certificazione di terze parti, che ti invia tutti i dettagli del certificato direttamente in un'email confidenziale. Dopo il ricevimento di tale email, hai l'opzione di [importare i certificati SSL](import-ssl-certificate.html) in {{site.data.keyword.slportal_full}} dovrebbe farti scegliere di usare il certificato con {{site.data.keyword.BluSoftlayer_full}} prodotti e servizi. Poiché {{site.data.keyword.cloud_notm}} non riceve mai i dettagli del certificato SSL, i dati non possono essere importati automaticamente.

## Cos'è un certificato SSL?

I certificati SSL sono abilitati da siti web come misura di sicurezza per proteggere l'utente. Sono generalmente utilizzati quando si devono trasmettere informazioni riservate a un sito web, come nome, indirizzo, numero di carta di credito e altri dati personali o gestiscono dati che richiedono l'autenticazione (come in {{site.data.keyword.slportal}}). I certificati SSL sono richiesti dalla società che gestisce il sito web ma vengono emessi da una società attendibile di terze parti che garantisce la validità del sito. I siti web protetti sono preceduti da HTTPS nell'URL, invece dello standard HTTP.

## Come posso ordinare un SSL SHA2?

Se hai già ordinato un SSL che mostra gli errori che il certificato SSL sta utilizzando SHA-1 invece di SHA-2, devi richiedere che il SSL venga riemesso. Puoi farlo inviando un ticket.

Se non hai ancora ordinato un SSL da {{site.data.keyword.cloud_notm}} e devi ordinarne uno con SHA-2, inoltra un ticket per ordinare manualmente un SSL per il dominio in questione. {{site.data.keyword.slportal}} crea ancora automaticamente certificati SSL che utilizzano SHA-1, se quindi lo utilizzi, dovrai poi fartelo riemettere.
