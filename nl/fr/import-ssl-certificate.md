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

# Importer des certificats SSL
{: #importing-ssl-certificates}

Une fois qu'un certificat SSL est émis pour un site web, il peut être importé dans la console {{site.data.keyword.cloud}}. En important des certificats SSL dans la console {{site.data.keyword.cloud_notm}}, vous pouvez les appliquer aux produits et services qui peuvent en avoir besoin, tels que la fonction de [déchargement SSL](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer) des équilibreurs de charge. Par défaut, les certificats SSL émis par {{site.data.keyword.cloud_notm}} ne sont pas importés dans la liste, car seul leur destinataire est censé les manipuler. Par conséquent, tout certificat SSL utilisé avec un produit ou service {{site.data.keyword.cloud_notm}} doit être importé manuellement par un utilisateur autorisé du compte. {:shortdesc}

## Importer des certificats SSL

Pour importer un certificat SSL, procédez comme indiqué ci-après.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Cliquez sur **Importer le certificat SSL**. 
4. Entrez les **détails du certificat SSL** dans les zones prévues à cet effet, puis cliquez sur **Importer**. Pour plus d'informations, reportez-vous au tableau ci-dessous. 

   Les détails que vous entrez dans la fenêtre **Importer le certificat SSL** doivent reproduire fidèlement (espaces et sauts de ligne compris) les données qui vous ont été communiquées par l'autorité de certification. Dans le cas contraire, une erreur se produira.
   {:note}

| Détails d'un certificat SSL | Description |
| --------------------------- | ----------- |
|Certificat                  | Détails du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Clé privée                  | Détails de la clé privée du certificat, fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Certificat intermédiaire    | Détails du certificat intermédiaire fournis par l'autorité de certification. Les certificats intermédiaires ne sont pas requis. Cependant, si les informations sont disponibles pour le certificat SSL, elles doivent être entrées.|
|Demande de signature de certificat | Détails de la demande de signature de certificat (CSR) fournis par l'autorité de certification. Ces détails ne sont pas requis, mais ils doivent être fournis s'ils font partie du certificat. **Remarque :** La demande de signature de certificat ne doit être changée en aucune manière. Une clé publique peut être incluse avec la demande. Elle ne doit pas être remplacée par la clé privée.|
|Remarques                        | Toutes notes concernant le certificat SSL qui peuvent être utiles aux autres utilisateurs.|
{: caption="Tableau 1. Détails d'un certificat SSL" caption-side="top"}

## Etapes suivantes

Une fois qu'il a été importé dans la console {{site.data.keyword.cloud_notm}}, le certificat SSL est stocké et demeure visible dans l'écran Certificats SSL jusqu'à ce qu'il soit [supprimé manuellement](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). Il sera proposé dans la liste des certificats SSL disponibles et utilisables, pour tous les produits ou services nécessitant un tel certificat. Vous pouvez le [mettre à jour](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) et les détails le concernant peuvent être, à tout moment, [téléchargés en toute sécurité](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details).
