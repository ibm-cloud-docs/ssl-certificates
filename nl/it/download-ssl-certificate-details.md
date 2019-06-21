---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Dettagli sullo scaricamento del certificato SSL
{: #downloading-ssl-certificate-details}

Dopo che un certificato SSL viene aggiunto alla console {{site.data.keyword.cloud}}, i suoi dettagli possono essere scaricati in ogni momento. Gli scaricamenti possono includere il certificato, la chiave o il PEM, che include tutti i dettagli disponibili associati al certificato SSL. I dettagli del certificato SSL sono scaricati in sicurezza, quindi non ci sono rischi associati al recupero dei dettagli con questo metodo.
{:shortdesc}

Per scaricare i dettagli per il certificato SSL, completa la seguente procedura.

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **SSL > Certificati**.
3. Dal menu **Azioni** seleziona le **Opzioni di scaricamento** preferite per il certificato. Consulta la seguente tabella per ulteriori informazioni:

| Opzioni di scaricamento      | Informazioni di scaricamento |
| -------------------- | -------------------- |
| Scarica certificato | Scarica solo la parte del certificato e non include la chiave privata, il certificato intermedio, la richiesta firma certificato (CSR) o i dettagli delle note. |
| Scarica chiave         | Scarica solo la chiave privata e non include il certificato, il certificato intermedio, la richiesta firma certificato (CSR) o i dettagli delle note. |
| Scarica PEM         | Scarica tutti i dettagli che sono associati al certificato SSL, incluso il certificato, la chiave privata, il certificato intermedio, la richiesta firma certificato (CSR) e i dettagli delle note. |
{: caption="Tabella 1. Opzioni di scaricamento" caption-side="top"}

## Fasi successive

Dopo la richiesta di scaricare i dettagli del certificato SSL, essi vengono automaticamente scaricati nel browser web. Seleziona lo scaricamento per aprire il file. Il file può anche essere salvato nella tua postazione di lavoro per il futuro; tuttavia, i dati di ogni certificato SSL presente nella schermata dei certificati SSL possono essere scaricati automaticamente in qualsiasi momento ripetendo i passi precedenti.

