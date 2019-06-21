---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Richiedere un'email di adempimento ordine del certificato SSL
{: #requesting-an-ssl-certificate-fulfillment-email}

Dopo l'ordinazione di un nuovo certificato SSL tramite {{site.data.keyword.cloud}}, l'autorità di certificazione invia un'email di adempimento ordine all'amministratore del dominio fornito durante il processo di ordinazione. Questa email contiene tutti i dettagli associati al certificato SSL. In ogni momento l'email di adempimento ordine può essere richiesta nuovamente dalla schermata ordini SSL nella console {{site.data.keyword.cloud_notm}}.
{:shortdesc}

## Richiesta dell'email di adempimento ordine
Completa la seguente procedura per richiedere l'email di adempimento ordine SSL dall'autorità di certificazione.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Ordini**.
3. Fai clic su **Invia** nella colonna **Email** per il certificato SSL che desideri.

  Viene visualizzata una finestra a comparsa per confermare la richiesta. Questa finestra contiene l'indirizzo email dell'amministratore del dominio fornito quando il certificato SSL è stato richiesto.
  {:note}

4. Fai clic su **Invia nuovamente email** per confermare la selezione e richiedere un'ulteriore email di adempimento ordine dall'autorità di certificazione.

## Fasi successive

Dopo la richiesta di un'ulteriore email di adempimento ordine, la richiesta verrà inoltrata all'autorità di certificazione applicabile per il completamento. Dato che i dettagli del certificato SSL sono confidenziali, {{site.data.keyword.cloud_notm}} non memorizza i dati del certificato SSL nel suo sistema. Dopo il ricevimento dei dettagli del certificato SSL tramite email, possono essere manualmente [importati](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) nella console {{site.data.keyword.cloud_notm}}, se necessario.
