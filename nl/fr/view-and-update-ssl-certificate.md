---
copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizzazione e aggiornamento dei certificati SSL

Dopo che un certificato SSL viene importato nella schermata dei certificati SSL, puoi visualizzarlo e aggiornarlo in qualsiasi momento. Il lavoro di aggiornamento analogo al [processo di importazione](import-ssl-certificate.html), così come tutti i dettagli che vengono aggiornati, devono coincidere esattamente con il certificato originale, inclusi la spaziatura e le interruzioni di linea.

Per visualizzare e aggiornare un certificato SSL, completa la seguente procedura.

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando credenziali univoche.
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
2. Seleziona **Visualizza/Aggiorna certificato** dall'elenco a discesa **Azioni**.
3. Aggiorna i **dettagli del certificato SSL** nelle caselle di testo applicabile.

   **Nota:** i dettagli che vengono immessi nella finestra **Importa certificato SSL** devono essere immessi esattamente come vengono forniti dall'autorità di certificazione, inclusi la spaziatura e le interruzioni di linea. Se ciò non accade si verifica un errore.

| Dettagli del certificato SSL | Descrizione |
| --------------------------- | ----------- |
|Certificato                  | I dettagli del certificato SSL, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Chiave privata                  | I dettagli della chiave privata del certificato, forniti dall'autorità di certificazione. Generalmente sono blocchi di testo alfanumerici.|
|Certificato intermedio     | I dettagli del certificato intermedio, forniti dall'autorità di certificazione. I certificati intermedi non sono necessari, tuttavia, se le informazioni sono disponibili per il certificato SSL, dovrebbero essere immessi.|
|Richiesta di firma del certificato  | I dettagli di CSR (Certificate Signing Request), forniti dall'autorità di certificazione. I dettagli CSR non sono necessari ma dovrebbero essere forniti se sono parte del certificato. **Nota:** non modificare il CSR in alcun modo. Una chiave pubblica può essere inclusa con il CSR e non deve essere sostituita dalla chiave privata.|
|Note                        | Ogni nota riguardante il certificato SSL che potrebbe essere utile ad altri utenti.|
{: caption="Tabella 1. Dettagli del certificato SSL " caption-side="top"}

Fai clic su **Aggiorna** per aggiornare il certificato SSL o fai clic su **Annulla** per annullare l'azione.

## Passi successivi

Dopo aver aggiornato i dettagli del certificato SSL, ogni prodotto o servizio che utilizza il certificato non verrà negativamente impattato dalla modifica. Il certificato può essere aggiornato nuovamente ed in ogni momento ripetendo i passi precedenti.
