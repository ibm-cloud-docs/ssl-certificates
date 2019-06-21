---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renouveler des certificats SSL
{: #renewing-ssl-certificates}

Une fois qu'un certificat SSL a été commandé via {{site.data.keyword.cloud}}, il est possible de le renouveler à tout moment. {{site.data.keyword.cloud_notm}} agit en tant que facilitateur entre l'autorité de certification et vous-même, et ne voit ni ne contrôle aucune partie du processus de renouvellement qui implique les détails du certificat SSL. Les certificats SSL sont renouvelés selon les mêmes termes que dans leur commande précédente, de sorte qu'aucun changement ne peut être apporté aux détails du renouvellement (type de certificat et autorité de certification, mois de validité, plateforme serveur, etc.). Un certificat peut être renouvelé avant ou après son expiration. Cependant, pour qu'un certificat SSL soit valide sans interruption, pensez à le renouvelez avant sa date d'expiration.
{:shortdesc}

## Renouveler un certificat SSL
Pour renouveler un certificat SSL, procédez comme indiqué ci-après.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Commandes**.
3. Cliquez sur **Renouveler** dans la colonne **Renouveler**, sur la ligne du certificat SSL voulu.
4. Déterminez si tous les détails du renouvellement et de la demande de signature de certificat sont corrects avant de renouveler le certificat SSL. Pour plus d'informations, reportez-vous au tableau ci-dessous.   

| Détails                         | Action  |
| ------------------------------- | ------- |
| Détails du renouvellement et de la demande de signature de certificat corrects | Sélectionnez **Renouveler** pour renouveler le certificat SSL. |
| Détails du renouvellement incorrects       | Sélectionnez **Achetez un nouveau certificat SS** pour commander un nouveau certificat. Les détails d'un certificat renouvelé, en particulier son type, l'autorité de certification et l'adresse e-mail du valideur, ne pouvant pas être modifiés, le seul moyen de changer les détails du certificat SSL d'un site Web consiste à commander un nouveau certificat. |
| Détails de la demande de signature de certificat corrects           | Sélectionnez **Modifier demande de signature de certificat**, entrez les détails de la nouvelle demande de signature de certificat dans la **zone de texte CSR**, puis sélectionnez **Restaurer demande de signature de certificat**. |
{: caption="Tableau 1. Détails du renouvellement et de la demande de signature de certificat" caption-side="top"}

## Etapes suivantes

Une fois que vous avez demandé le renouvellement d'un certificat SSL, {{site.data.keyword.cloud_notm}} transfère votre demande à l'autorité de certification afin qu'elle effectue les vérifications du site Web nécessaires au renouvellement. Une fois que le certificat a été renouvelé, sa nouvelle date d'expiration s'affiche dans la zone **Expiration**. 
