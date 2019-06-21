---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: SSL certificate, SSL technology, public key

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introduzione alla tecnologia SSL
{: #introduction-to-ssl-technology}

Secure Sockets Layer (SSL) è una tecnologia che crittografa il traffico tra l'applicazione client e il server delle applicazioni. Questa crittografia viene eseguita utilizzando una chiave pubblica/chiave privata di sistema che utilizza un certificato SSL. Il certificato SSL contiene la chiave pubblica del server, le date di validità del certificato, un nome host per cui il certificato è valido e una firma dall'autorità di certificazione che lo ha emesso.
{:shortdesc}

## Terminologia SSL

I certificati SSL hanno una terminologia univoca. Potresti incontrare i seguenti termini mentre lavori con i certificati SSL.

### Dimensione bit
Le chiavi di crittografia vengono misurate in base alla loro dimensione in bit. Ad esempio, 512 bit, 1024 bit, 2048 bit. Generalmente una chiave più lunga sarà più lenta da utilizzare ma più sicura. Attualmente la dimensione minima per le chiavi che vengono utilizzate nei certificati SSL è 1024 bit, sebbene i certificati di convalida estesa richiedano 2048 bit.

### Catena di certificati
I certificati SSL non vengono generalmente utilizzati da soli. Nella maggior parte delle implementazioni si ha a che fare con una catena di certificati. Ad esempio:

    Root > intermediate1 > server cert.

    \> Intermediate2 > server2 cert

In questo esempio, il certificato del server viene firmato dal certificato intermedio, che è a sua volta firmato dal certificato root. Il concatenamento in questo modo può rendere l'SSL più sicuro perché significa che il certificato root non viene utilizzato (ed esposto a rischio) così spesso. Se `intermediate1` è stato compromesso, allora `server cert` potrebbe essere in pericolo ma `server2 cert` potrebbe andare bene perché sono parti di catene differenti.

### CSR (Certificate Signing Request) 
Il CSR (Certificate Signing Request) è un documento che si genera sul server e che contiene informazioni che l'autorità di certificazione utilizza per creare il certificato corrente.

### Nome comune
Il nome comune (CN) è il nome host per cui il certificato è valido (ad esempio, www.domain.com).  

 www.domain.com, smtp.domain.com e mail.domain.com sono tre nomi host differenti e lo stesso certificato SSL non è valido per tutti e tre (a meno che non si stia utilizzando un certificato jolly, ma attualmente {{site.data.keyword.cloud}} non lo offre).
 {:note}

### Chiave privata/pubblica
SSL utilizza una tecnica denominata crittografia chiave pubblica. In questo formato di crittografia hai due chiavi: la pubblica e la privata. La chiave pubblica è distribuita in lungo e in largo. Nessuno vede la tua chiave privata. Chi vuole comunicare in modo sicuro con te crittografa la comunicazione attraverso la tua chiave pubblica. La crittografia chiave pubblica è basata sulla asserzione che i bit crittografati con una chiave pubblica specificata possono essere decodificati solo utilizzando la corrispondente chiave privata e viceversa.

### Certificato root
I certificati root SSL sono certificati che si firmano da soli e vengono presentati al mondo dalle rispettive autorità di certificazione. I certificati root per le autorità di certificazione sono già installati nell'archivio certificati del tuo browser web. Questo consente al tuo browser di ritenere attendibili questi certificati e formare l'inizio della catena di attendibilità che porta alla fine al certificato che hai installato sul server.

### Firma 
I certificati SSL hanno una firma digitale che è inserita dall'autorità di certificazione. Questa firma, quando è riconducibile ad un certificato root attendibile, conferma l'autenticità del certificato.

## SSL nell'infrastruttura IBM Cloud

{{site.data.keyword.cloud}} rivende tre tipi di certificati SSL: convalida del dominio, convalida dell'organizzazione e convalida estesa.

I certificati di convalida del dominio (DV) sono economici e disponibili velocemente. La convalida che viene eseguita dall'autorità di certificazione è limitata a inviare un'email ad un indirizzo email specificato nel dominio in questione e ottenere una risposta positiva. I certificati di convalida dell'organizzazione (OV) e di convalida estesa (EV) impiegano un paio di giorni (a volte una settimana), costano di più e comportano controlli più approfonditi dall'autorità di certificazione. I certificati EV sono codificati in modo che i browser li riconoscono come EV e visualizzano una barra verde come parte della barra dell'indirizzo.

I certificati SSL, come altri servizi {{site.data.keyword.cloud_notm}}, possono essere gestiti tramite la console {{site.data.keyword.cloud_notm}}. Vai al menu **Sicurezza** e seleziona l'opzione **SSL** per ordinare e gestire i certificati.  

I certificati SSL ordinati tramite {{site.data.keyword.cloud_notm}} non devono essere utilizzati su un server {{site.data.keyword.cloud_notm}}. Inoltre i certificati ordinati altrove possono essere utilizzati sui tuoi server che sono ospitati qui.
{:note}

I certificati SSL migliorano la sicurezza delle transazioni e forniscono agli utenti un senso di sicurezza. Oltre ai certificati SSL la sicurezza daemon, la sicurezza fisica, le procedure di codifica e la gestione del certificato si combinano per creare un profilo di sicurezza globale della soluzione.

