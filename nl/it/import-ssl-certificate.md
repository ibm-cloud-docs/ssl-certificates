---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importazione di certificati SSL
{: #importing-ssl-certificates}

Dopo che un certificato SSL viene emesso per un sito Web, può essere importato nella console {{site.data.keyword.cloud}}. Con l'importazione dei certificati SSL nella console {{site.data.keyword.cloud_notm}}, i certificati possono essere applicati a prodotti e servizi che potrebbero richiederli, come [SSL offloading](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer) del programma di bilanciamento del carico. Per impostazione predefinita, i certificati SSL che vengono emessi da {{site.data.keyword.cloud_notm}} non vengono importati nell'elenco, in quanto sono destinati a essere manipolati solo dal destinatario. Pertanto, qualsiasi certificato SSL utilizzato con un {{site.data.keyword.cloud_notm}} prodotto o servizio deve essere importato manualmente da un utente autorizzato nell'account. {:shortdesc}

## Importazione di certificati SSL

Completa la seguente procedura per importare un certificato SSL.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Fai clic su **Importa certificato SSL**.
4. Immetti i **dettagli del certificato SSL** nei campi applicabili e fai clic su **Importa.** Per ulteriori informazioni, consulta la seguente tabella.

   I dettagli che vengono immessi nella finestra **Importa certificato SSL** devono essere immessi esattamente come vengono forniti dall'autorità di certificazione, incluse la spaziatura e le interruzioni di linea. Se ciò non accade si verifica un errore.
   {:note}

| Dettagli del certificato SSL     | Descrizione |
| --------------------------- | ----------- |
|Certificato                  | I dettagli del certificato SSL, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Chiave privata                  | I dettagli della chiave privata del certificato, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Certificato intermedio     | I dettagli del certificato intermedio, forniti dall'autorità di certificazione. I certificati intermedi non sono necessari; tuttavia, se le informazioni sono disponibili per il certificato SSL, dovrebbero essere immessi.|
|CSR (Certificate Signing Request) | I dettagli di CSR (Certificate signing request) forniti dall'autorità di certificazione. I dettagli CSR non sono necessari ma dovrebbero essere forniti se sono parte del certificato. **Nota:** non modificare il CSR in alcun modo. Una chiave pubblica può essere inclusa con il CSR e non deve essere sostituita dalla chiave privata.|
|Note                        | Ogni nota riguardante il certificato SSL che potrebbe essere utile ad altri utenti.|
{: caption="Tabella 1. Dettagli del certificato SSL" caption-side="top"}

## Fasi successive

Dopo che il certificato SSL viene importato nella console {{site.data.keyword.cloud_notm}}, viene memorizzato nella schermata dei certificati SSL finché non viene [eliminato manualmente](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). Per tutti i prodotti o i servizio che richiedo i dettagli del certificato SSL, il nuovo certificato SSL appare nell'elenco dei certificati disponibili all'uso quando si interagisce con la funzione SSL del prodotto o servizio desiderato. Il certificato può essere [aggiornato](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) ed i dettagli sul certificato possono essere [scaricati in modo sicuro](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) in ogni momento.
