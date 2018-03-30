---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Attivazione o disattivazione dell'accesso VPN PPTP

VPN PPTP consente agli utenti di creare un tunnel sicuro sulla {{site.data.keyword.BluSoftlayer_full}} rete privata utilizzando il software client specializzato in esecuzione sul loro desktop o dispositivo dedicato. L'accesso PPTP è progettato per i clienti che devono collegare un intero ufficio o non possono utilizzare la soluzione VPN SSL. Ad ogni cliente è destinata una connessione PPTP con ulteriori connessioni disponibile ma che richiedono supporto per abilitare l'accesso PPTP illimitato, che é disponibile senza costi aggiuntivi. Per attivare o disattivare l'accesso VPN PPTP per un utente, completa la seguente procedura.

1. Accedi alla [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} utilizzando le tue credenziali univoche da amministratore.
2. Individua l'utente il cui accesso vuoi modificare e visualizza la colonna **Accesso VPN** per visualizzare il livello di accesso corrente.
3. Dal menu **Azioni**, seleziona **Modifica accesso VPN**.
4. Immetti il tipo VPN ed i dettagli di accesso alla sottorete.

|Nome campo |Opzioni   |
| -----------| ------------ |
| Tipo VPN   | Nessuno, SSL, PPTP o entrambi (SSL e PPTP) |
|Accesso alla sottorete | Automatico o Manuale |           
{: caption="Tabella 1. Modifica delle opzioni di accesso VPN" caption-side="top"}   
5. Fai clic su **Salva** per salvare le modifiche.

   **Nota:** l'accesso PPTP deve essere attivato per consentire all'utente di connettersi utilizzando PPTP.
