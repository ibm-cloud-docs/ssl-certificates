---
copyright:
  years: 2014, 2018
lastupdated: "2018-06-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importazione di certificati SSL

Dopo che un certificato SSL viene emesso per un sito Web, può essere importato in {{site.data.keyword.slportal_full}}. Con l'importazione dei certificati SSL in {{site.data.keyword.slportal}}, i certificati possono essere applicati a prodotto e servizi che potrebbero richiederli, come [SSL Offloading](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window} del programma di bilanciamento del carico. Per impostazione predefinita, i certificati SSL che vengono emessi da {{site.data.keyword.BluSoftlayer_full}} non vengono importati nell'elenco, in quanto sono destinati a essere manipolati solo dal destinatario. Pertanto, qualsiasi certificato SSL da utilizzare con un {{site.data.keyword.BluSoftlayer_notm}} prodotto o servizio deve essere importato manualmente da un utente autorizzato nell'account. Completa la seguente procedura per importare un certificato SSL in {{site.data.keyword.slportal}}.

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Fai clic su **Importa certificato SSL**.
4. Immetti i **dettagli del certificato SSL** nei campi applicabili e fai clic su **Importa.**

   **Nota:** i dettagli che vengono immessi nella finestra **Importa certificato SSL** devono essere immessi esattamente come vengono forniti dall'autorità di certificazione, inclusi la spaziatura e le interruzioni di linea. Se ciò non accade si verifica un errore.

| Dettagli del certificato SSL | Descrizione |
| --------------------------- | ----------- |
|Certificato                  | I dettagli del certificato SSL, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Chiave privata                  | I dettagli della chiave privata del certificato, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Certificato intermedio     | I dettagli del certificato intermedio, forniti dall'autorità di certificazione. I certificati intermedi non sono necessari, tuttavia, se le informazioni sono disponibili per il certificato SSL, dovrebbero essere immessi.|
|Richiesta di firma del certificato  | I dettagli di CSR (Certificate Signing Request), forniti dall'autorità di certificazione. I dettagli CSR non sono necessari ma dovrebbero essere forniti se sono parte del certificato. **Nota:** non modificare il CSR in alcun modo. Una chiave pubblica può essere inclusa con il CSR e non deve essere sostituita dalla chiave privata.|
|Note                        | Ogni nota riguardante il certificato SSL che potrebbe essere utile ad altri utenti.|
{: caption="Tabella 1. Dettagli del certificato SSL " caption-side="top"}

## Passi successivi

Dopo che il certificato SSL viene importato in {{site.data.keyword.slportal}}, viene memorizzato nella schermata dei certificati SSL fino a che non venga [eliminato manualmente](delete-ssl-certificate.html). Per tutti i prodotti o i servizio che richiedo i dettagli del certificato SSL, il nuovo certificato SSL appare nell'elenco dei certificati disponibili all'uso quando si interagisce con la funzione SSL del prodotto o servizio desiderato. Il certificato può essere [aggiornato](view-and-update-ssl-certificate.html) ed i dettagli sul certificato possono essere [scaricati in modo sicuro](download-ssl-certificate-details.html) in ogni momento.
