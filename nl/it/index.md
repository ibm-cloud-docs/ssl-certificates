---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Esercitazione introduttiva
{: #getting-started-tutorial}

## Prima di cominciare

L'introduzione a SSL richiede un po' di pianificazione. Completa i seguenti prerequisiti.

1. Decidi dove ottenere il certificato
2. Informati sui tipi di certificati, la lunghezza della chiave e la durata
3. Scegli un nome comune
4. Informati sulle regole socket
5. Genera il CSR

Per ulteriori informazioni, vedi [Pianificazione per i certificati SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## Ordine dei certificati SSL

1. Vai al menu di sicurezza della tua console. Per ulteriori informazioni, vedi [Passaggio ai dispositivi](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Dal menu **Sicurezza** seleziona **Sicurezza > SSL > Certificati**.
3. Seleziona **Ordina certificato SSL**.
3. Seleziona il tipo e la durata del certificato, invia il testo del CSR, seleziona la tua piattaforma del server e conferma quindi il pagamento.

## Installazione e verifica
Dopo che i processi di ordinazione e verifica vengono completati, riceverai un'email dall'autorità di certificazione che include il tuo certificato così come ogni certificato intermedio necessario. Il metodo per l'installazione dipende dal software che stai utilizzando ma il risultato dovrebbe essere lo stesso. Una volta completato, dovresti essere in grado di andare in `http://host.yourdomain.com` e vedere il tuo contenuto mentre vedi anche il lucchetto SSL che i browser utilizzano per indicare una sessione crittografata. Se ottieni un avviso, allora esistono passi che devi eseguire.

## Fasi successive

Dopo una corretta verifica, puoi accedere ai tuoi certificati SSL nella console {{site.data.keyword.cloud_notm}} per [aggiornare](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [scaricare](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [eliminare](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) o [importare](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) certificati SSL esistenti nello strumento.
