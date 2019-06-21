---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Attivazione o disattivazione dell'accesso VPN PPTP
{: #activating-or-deactivating-pptp-vpn-access}

VPN PPTP ti consente di creare un tunnel sicuro sulla {{site.data.keyword.cloud}} rete privata utilizzando il software client specializzato in esecuzione sul tuo desktop o dispositivo dedicato. L'accesso PPTP è progettato se devi connettere un intero ufficio o non puoi utilizzare la soluzione VPN SSL. Ti viene destinata una connessione PPTP con ulteriori connessioni disponibili e puoi richiedere supporto per abilitare l'accesso PPTP illimitato, che è disponibile senza costi aggiuntivi. Per attivare o disattivare l'accesso VPN PPTP per un utente, completa la seguente procedura.
{:shortdesc}

1. Accedi alla pagina [Accesso (IAM)](https://cloud.ibm.com/iam/overview){: external} nella console {{site.data.keyword.cloud_notm}}.
2. Individua l'utente il cui accesso vuoi modificare e visualizza la colonna **Accesso VPN** per visualizzare il livello di accesso corrente.
3. Dal menu **Azioni**, seleziona **Modifica accesso VPN**.
4. Immetti il tipo VPN ed i dettagli di accesso alla sottorete e fai clic su **Salva** per salvare le tue modifiche. Per ulteriori informazioni, consulta la seguente tabella.

|Nome campo  |Opzioni   |
| -----------| ------------ |
| Tipo VPN   | Nessuno, SSL, PPTP o entrambi (SSL e PPTP) |
| Accesso alla sottorete | Automatico o Manuale |           
{: caption="Tabella 1. Dettagli VPN e sottorete" caption-side="top"}   

L'accesso PPTP deve essere attivato per consentire all'utente di connettersi utilizzando PPTP.
{:note}
