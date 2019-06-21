---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Demander l'e-mail d'exécution d'un certificat SSL
{: #requesting-an-ssl-certificate-fulfillment-email}

Lorsque vous passez commande d'un nouveau certificat SSL via {{site.data.keyword.cloud}},
l'autorité de certification envoie un e-mail d'exécution à l'administrateur de domaine dont les coordonnées sont fournies dans cette commande. Cet e-mail contient tous les détails associés au certificat SSL. Vous pouvez à tout moment demander un nouvel envoi de l'e-mail d'exécution d'un certificat particulier à partir de l'écran Commandes SSL de la console {{site.data.keyword.cloud_notm}}. {:shortdesc}

## Demander un e-mail d'exécution
Pour demander à l'autorité de certification qu'elle vous renvoie l'e-mail d'exécution d'un certificat SSL, procédez comme indiqué ci-après.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Commandes**.
3. Cliquez sur **Envoyer** dans la colonne **E-mail**, sur la ligne du certificat SSL voulu. 

  Une fenêtre apparaît pour vous permettre de confirmer votre demande. Cette fenêtre contient l'adresse e-mail de l'administrateur de domaine qui a été communiquée lors de la commande du certificat SSL. {:note}

4. Cliquez sur **Renvoyer l'e-mail** pour confirmer votre choix et demander que l'autorité de certification vous envoie un nouvel exemplaire de l'e-mail d'exécution.

## Etapes suivantes

Une fois que vous avez demandé à recevoir un nouvel exemplaire de l'e-mail d'exécution, votre demande est
transférée à l'autorité de certification compétente afin qu'elle y réponde. Les détails d'un certificat SSL étant confidentiels, {{site.data.keyword.cloud_notm}} ne les stocke pas sur ses systèmes. Une fois les détails du certificat SSL reçus par e-mail ils peuvent, au besoin, être [importés](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) manuellement dans la console {{site.data.keyword.cloud_notm}}.
