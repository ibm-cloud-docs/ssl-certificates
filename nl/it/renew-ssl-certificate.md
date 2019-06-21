---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Rinnovare i certificati SSL
{: #renewing-ssl-certificates}

Dopo che un certificato SSL viene ordinato tramite {{site.data.keyword.cloud}}, può essere rinnovato in qualsiasi momento. Durante il processo di rinnovo, {{site.data.keyword.cloud_notm}} funge da mediatore tra il cliente (tu) e l'autorità di certificazione (CA), e non vede o controlla nessuna parte del processo di rinnovo che coinvolge i dettagli del certificato SSL. I certificati SSL vengono rinnovati negli stessi termini in cui sono stati ordinati, quindi nessuna modifica ai dettagli di rinnovo (tipo di certificato e autorità, mese di validità, piattaforma del server e così via) può essere fatta. I certificati possono essere rinnovati prima o dopo la scadenza; tuttavia, per mantenere la validità del certificato SSL, rinnova il certificato prima della sua data di scadenza.
{:shortdesc}

## Rinnovo di un certificato SSL
Completa la seguente procedura per rinnovare un certificato SSL.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Ordini**.
3. Fai clic su **Rinnova** nella colonna **Rinnova** per il certificato SSL desiderato.
4. Determina se tutti i dettagli di rinnovo e CSR sono corretti prima di rinnovare il certificato SSL. Per ulteriori informazioni, consulta la seguente tabella.  

|Dettagli|Azione|
| ------------------------------- | ------- |
| Dettagli CSR e rinnovo corretti | Seleziona **Rinnova** per rinnovare il certificato SSL. |
| Dettagli rinnovo non corretti       | Seleziona **Acquista un nuovo certificato SSL** per ordinare un nuovo certificato. Poiché i dettagli del rinnovo, incluso il tipo di certificato, l'autorità e l'email di approvazione non possono essere modificati, l'unico modo per aggiornare i dettagli del certificato SSL di un sito web è di ordinare un nuovo certificato.|
| Dettagli CSR non corretti           | Seleziona **Modifica CSR**, immetti i nuovi dettagli CSR nella **casella di testo CSR** e seleziona **Ripristina CSR**. |
{: caption="Tabella 1. Dettagli sul rinnovo e su CSR" caption-side="top"}

## Fasi successive

Dopo la richiesta di rinnovo di un certificato SSL, {{site.data.keyword.cloud_notm}} inoltra la richiesta sull'autorità di certificazione per completare la verifica del sito web obbligatoria per il rinnovo. Al rinnovo del certificato, la nuova data di scadenza appare nel campo **Scadenza**.
