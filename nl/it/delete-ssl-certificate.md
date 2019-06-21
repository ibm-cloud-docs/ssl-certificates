---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Eliminazione dei certificati SSL
{: #deleting-ssl-certificates}

Dopo che i dettagli di un certificato SSL vengono importati nella console {{site.data.keyword.cloud}}, può essere eliminato in qualsiasi momento per impedire a tutti i dati di essere salvati nella console {{site.data.keyword.cloud_notm}}.

Per eliminare un certificato SSL, completa la seguente procedura.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Dal menu **Azioni** seleziona **Elimina** per il certificato SSL desiderato.
4. Fai clic su **Sì** per eliminare il certificato SSL. 

## Fasi successive

Dopo l'eliminazione di un certificato SSL, tutti i servizi che sono collegati al certificato non utilizzano più le sue informazioni. Il certificato non appare più nella schermata dei certificati SSL all'interno della console {{site.data.keyword.cloud_notm}}.

Aggiorna tutti i servizi che in precedenza utilizzavano il certificato eliminato per essere associati a un certificato SSL valido che è associato all'account.

In ogni momento il certificato SSL può essere nuovamente aggiunto alla console {{site.data.keyword.cloud_notm}} utilizzando il processo [importa](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates).
{:note}
