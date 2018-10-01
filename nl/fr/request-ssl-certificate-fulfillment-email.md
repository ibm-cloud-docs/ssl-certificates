---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Richiedere un'email di adempimento ordine del certificato SSL

Dopo l'ordinazione di un nuovo certificato SSL tramite {{site.data.keyword.BluSoftlayer_full}}, l'autorità di certificazione invia un'email di adempimento ordine all'amministratore del dominio fornito durante il processo di ordinazione. Questa email contiene tutti i dettagli associati al certificato SSL. In ogni momento l'email di adempimento ordine può essere richiesta nuovamente dalla schermata ordini SSL in {{site.data.keyword.slportal_full}}. Completa la seguente procedura per richiedere l'email di adempimento ordine SSL dall'autorità di certificazione.

## Richiesta dell'email di adempimento ordine

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Dal menu **Sicurezza** seleziona **SSL > Ordini**.
3. Fai clic sul collegamento **Invia** nella colonna **Email** per il certificato SSL che desideri.<br/>**Nota:** viene visualizzata una finestra a comparsa per confermare la richiesta. Questa finestra contiene l'indirizzo email dell'amministratore del dominio fornito quando il certificato SSL è stato richiesto.
4. Fai clic su **Invia nuovamente email** per confermare la selezione e richiedere un'ulteriore email di adempimento ordine dall'autorità di certificazione.  Oppure fai clic su **Annulla** per annullare l'azione.

## Passi successivi

Dopo la richiesta di un'ulteriore email di adempimento ordine, la richiesta verrà inoltrata all'autorità di certificazione applicabile per il completamento. Dato che i dettagli del certificato SSL sono confidenziali, {{site.data.keyword.BluSoftlayer_notm}} non memorizza i dati del certificato SSL nel suo sistema. Dopo il ricevimento dei dettagli del certificato SSL tramite email, possono essere manualmente [importati](import-ssl-certificate.html) in {{site.data.keyword.slportal}}, se necessario.
