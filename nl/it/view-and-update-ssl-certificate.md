---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizzazione e aggiornamento dei certificati SSL
{: #viewing-and-updating-ssl-certificates}

Dopo che un certificato SSL viene importato nella schermata dei certificati SSL, puoi visualizzarlo e aggiornarlo in qualsiasi momento. Il lavoro di aggiornamento analogo al [processo di importazione](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates), così come tutti i dettagli che vengono aggiornati, devono coincidere esattamente con il certificato originale, incluse la spaziatura e le interruzioni di linea.
{:shortdesc}

Per visualizzare e aggiornare un certificato SSL, completa la seguente procedura.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Seleziona **Visualizza/Aggiorna certificato** dall'elenco a discesa **Azioni**.
4. Aggiorna i **dettagli del certificato SSL** nelle caselle di testo applicabili e fai clic su **Aggiorna** per applicare le tue modifiche. Per ulteriori informazioni, consulta la seguente tabella.

   I dettagli che vengono immessi nella finestra **Importa certificato SSL** devono essere immessi esattamente come vengono forniti dall'autorità di certificazione, incluse la spaziatura e le interruzioni di linea. Se ciò non accade si verifica un errore.
   {:note}

| Dettagli del certificato SSL     | Descrizione |
| --------------------------- | ----------- |
|Certificato                  |I dettagli del certificato SSL forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Chiave privata                  | I dettagli della chiave privata del certificato forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Certificato intermedio     |I dettagli del certificato intermedio forniti dall'autorità di certificazione. I certificati intermedi non sono necessari; tuttavia, se le informazioni sono disponibili per il certificato SSL, dovrebbero essere immessi.|
|Richiesta di firma del certificato  | I dettagli di CSR (Certificate signing request) forniti dall'autorità di certificazione. I dettagli CSR non sono necessari ma dovrebbero essere forniti se sono parte del certificato. **Nota:** non modificare il CSR in alcun modo. Una chiave pubblica può essere inclusa con il CSR e non deve essere sostituita dalla chiave privata.|
|Note                        | Ogni nota riguardante il certificato SSL che potrebbe essere utile ad altri utenti.|
{: caption="Tabella 1. Dettagli del certificato SSL" caption-side="top"}

## Fasi successive

Dopo aver aggiornato i dettagli del certificato SSL, ogni prodotto o servizio che utilizza il certificato non verrà negativamente impattato dalla modifica. Il certificato può essere aggiornato nuovamente ed in ogni momento ripetendo i passi precedenti.
