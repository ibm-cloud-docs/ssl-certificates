---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# FAQ: certificati SSL
{: #faqs-ssl-certificates}

## Perché il certificato SSL che ho ordinato non viene visualizzato automaticamente nella schermata dei certificati SSL?
{:faq}

I certificati SSL vengono emessi da un'autorità di certificazione di terze parti, che ti invia tutti i dettagli del certificato direttamente in un'email confidenziale. Dopo il ricevimento di tale email, hai l'opzione di [importare i certificati SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) nella console {{site.data.keyword.cloud}}, dovresti scegliere di utilizzare il certificato con prodotti e servizi {{site.data.keyword.cloud_notm}}. Poiché {{site.data.keyword.cloud_notm}} non riceve mai i dettagli del certificato SSL, i dati non possono essere importati automaticamente.

## Cos'è un certificato SSL?
{:faq}

I certificati SSL sono abilitati da siti web come misura di sicurezza per proteggere l'utente. Sono generalmente utilizzati quando devi trasmettere informazioni riservate a un sito web, come nome, indirizzo, numero di carta di credito e altri dati personali o gestire i dati che richiedono l'autenticazione (come nella console {{site.data.keyword.cloud_notm}}). I certificati SSL sono richiesti dalla società che gestisce il sito web ma vengono emessi da una società attendibile di terze parti che garantisce la validità del sito. I siti web protetti sono preceduti da HTTPS nell'URL, invece dello standard HTTP.

## Come posso ordinare un SSL SHA2?
{:faq}

Se hai già ordinato un SSL che mostra gli errori che il certificato SSL sta utilizzando SHA-1 invece di SHA-2, devi richiedere che il SSL venga riemesso. Puoi farlo inviando un ticket.

Se non hai ancora ordinato un SSL da {{site.data.keyword.cloud_notm}} e devi ordinarne uno con SHA-2, inoltra un ticket per ordinare manualmente un SSL per il dominio in questione. La console {{site.data.keyword.cloud_notm}} crea ancora automaticamente i certificati SSL utilizzando SHA-1, per cui se fai in questo modo, dovrai poi farli riemettere.
