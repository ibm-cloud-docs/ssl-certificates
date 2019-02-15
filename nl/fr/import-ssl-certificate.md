---
copyright:
  years: 2014, 2018
lastupdated: "2018-06-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importer des certificats SSL

Une fois qu'un certificat SSL est émis pour un site web, il peut être importé dans
le portail {{site.data.keyword.slportal_full}}. En important des certificats SSL dans le portail {{site.data.keyword.slportal}}, vous pouvez
les appliquer aux produits et services qui peuvent en avoir besoin, tels que la fonction
de [déchargement SSL](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window} des équilibreurs de charge. Par défaut, les certificats SSL émis par {{site.data.keyword.BluSoftlayer_full}} ne sont pas importés dans la liste, car seul leur destinataire est censé les manipuler. Par conséquent, tout certificat SSL destiné à être utilisé avec un produit ou service {{site.data.keyword.BluSoftlayer_notm}} doit être importé manuellement par un utilisateur autorisé du compte. Pour importer un certificat SSL dans le portail {{site.data.keyword.slportal}}, procédez comme indiqué ci-après.

1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Cliquez sur **Importer le certificat SSL**.
4. Entrez les **détails du certificat SSL** dans les zones prévues à cet effet et cliquez sur **Importer**.

   **Remarque :** les détails que vous entrez dans la fenêtre **Importer le certificat SSL** doivent reproduire fidèlement (espaces et sauts de ligne compris) les données qui vous ont été communiquées par l'autorité de certification. Dans le cas contraire, une erreur se produira.

| Détails d'un certificat SSL     | Description |
| --------------------------- | ----------- |
|Certificat                  | Détails du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Clé privée                  | Détails de la clé privée du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Certificat intermédiaire     | Détails du certificat intermédiaire fournis par l'autorité de certification. Les certificats intermédiaires ne sont pas requis. Cependant, si les informations sont disponibles pour le certificat SSL, elles doivent être entrées.|
|Demande de signature de certificat  | Détails de la demande de signature de certificat (CSR) fournis par l'autorité de certification. Ces détails ne sont pas requis, mais ils doivent être fournis s'ils font partie du certificat. **Remarque :** La demande de signature de certificat ne doit être changée en aucune manière. Une clé publique peut être incluse avec la demande. Elle ne doit pas être remplacée par la clé privée.|
|Remarques                        | Toutes notes concernant le certificat SSL qui peuvent être utiles aux autres utilisateurs.|
{: caption="Tableau 1. Détails d'un certificat SSL" caption-side="top"}

## Etapes suivantes

Une fois importé sur le portail {{site.data.keyword.slportal}}, le certificat SSL est stocké et demeure visible dans l'écran Certificats SSL jusqu'à ce qu'il soit [supprimé manuellement](delete-ssl-certificate.html). Il sera proposé dans la liste des certificats SSL disponibles et utilisables, pour tous les produits ou services nécessitant un tel certificat. Vous pouvez le [mettre à jour](view-and-update-ssl-certificate.html) et les détails le concernant peuvent être, à tout moment, [téléchargés en toute sécurité](download-ssl-certificate-details.html).
