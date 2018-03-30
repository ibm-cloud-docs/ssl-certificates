---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Rinnovare i certificati SSL

Dopo che un certificato SSL viene ordinato tramite {{site.data.keyword.BluSoftlayer_full}}, può essere rinnovato in qualsiasi momento. Durante il processo di rinnovo, {{site.data.keyword.BluSoftlayer_notm}} funge da mediatore tra il cliente (tu) e l'autorità di certificazione, e non vede o controlla nessuna parte del processo di rinnovamento che coinvolge i dettagli del certificato SSL. I certificati SSL vengono rinnovati negli stessi termini in cui sono stati ordinati, quindi nessuna modifica ai dettagli di rinnovo (tipo di certificato e autorità, mese di validità, piattaforma del server e così via) può essere fatta. I certificati possono essere rinnovati prima o dopo la scadenza; tuttavia, per mantenere la validità del certificato SSL, rinnova il certificato prima della sua data di scadenza. Completa la seguente procedura per rinnovare un certificato SSL.

## Rinnovo di un certificato SSL

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Dal menu **Sicurezza** seleziona **SSL > Ordini**.
3. Fai clic sul collegamento **Rinnova** nella colonna **Rinnova** del il certificato SSL desiderato.

   **Nota:** una casella a comparsa apparirà per completare la richiesta.  
   * Determina se tutti i dettagli di rinnovo e il CSR siano corretti:<br /><br /><table border="1"><tr><th>Se...</th><th>Allora...</th></tr><tr><td>Tutti i dettagli di rinnovo e il CSR sono corretti</td><td>Passa alla fase successiva.</td></tr><tr><td>I dettagli di rinnovo non sono corretti</td><td><ul><li>Fai clic sul collegamento <strong>Acquista un nuovo certificato SSL</strong> per essere reindirizzato alla schermata di acquisto.<br /><blockquote><strong>Nota:</strong> poiché i dettagli di rinnovo, incluso il tipo di certificato, l'autorità e l'email di approvazione non possono essere modificati, l'unico modo per aggiornare i dettagli del sito web del certificato SSL è di ordinare un nuovo certificato.</blockquote></li><li>Completa le schermate sulla pagina dell'ordine con le informazioni desiderate per il certificato SSL. Nessuna azione aggiuntiva è necessaria utilizzando questa procedura.</li></ul></td></tr><tr><td>I dettaggli del CSR non sono corretti</td><td><ul><li>Fai clic sul pulsante **Cambia CSR**. </li><li>Immetti i **dettagli del nuovo CSR** nella casella di testo **CSR**.</li><li>Fai clic sul pulsante **Ripristina CSR**. </li></ul></td></tr></table>
4. Fai clic sul pulsante **Rinnova** per rinnovare il certificato SSL o clic su **Annulla** per annullare l'azione.

## Passi successivi

Dopo la richiesta di rinnovo di un certificato SSL, {{site.data.keyword.BluSoftlayer_notm}} inoltra la richiesta sull'autorità di certificazione per completare la verifica del sito web obbligatoria per il rinnovo. Al rinnovo del certificato, la nuova data di scadenza appare nel campo della scadenza.
