---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Eliminazione dei certificati SSL
{: #deleting-ssl-certificates}

Dopo che i dettagli di un certificato SSL vengono importati in {{site.data.keyword.slportal_full}}, può essere eliminato in qualsiasi momento per impedire a tutti i dati di essere salvati in {{site.data.keyword.slportal}}.

Per eliminare un certificato SSL, completa la seguente procedura.

1. Accedi alla [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Dal menu **Azioni** seleziona **Elimina** per il certificato SSL desiderato.

  **Nota:** appare una finestra per confermare l'eliminazione.
4. Fai clic su **Sì** per eliminare il certificato SSL o fai clic su **No** per annullare l'azione.

## Passi successivi

Dopo l'eliminazione di un certificato SSL, tutti i servizi che sono collegati al certificato non utilizzano più le sue informazioni. Il certificato non appare più nella schermata dei certificati SSL all'interno di {{site.data.keyword.slportal}}.

Si consiglia di aggiornare tutti i servizi che in precedenza utilizzavano il certificato eliminato per essere associati ad un certificato SSL valido che sia associato all'account.

**Nota:** in ogni momento il certificato SSL può essere nuovamente aggiunto a {{site.data.keyword.slportal}} utilizzando il processo [importa](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates).
