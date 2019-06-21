---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualisation et mise à jour des certificats SSL
{: #viewing-and-updating-ssl-certificates}

Une fois qu'un certificat SSL a été importé dans l'écran Certificats SSL, vous pouvez l'afficher et le mettre à jour à tout moment. Les mises à jour fonctionnent de manière similaire au [processus d'importation](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates). Tous les
détails mis à jour doivent correspondre exactement au certificat d'origine, y compris les espaces et les sauts de ligne.
{:shortdesc}

Pour voir et mettre à jour un certificat SSL, effectuez les étapes suivantes.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Sélectionnez **Afficher/mettre à jour le certificat** dans la
liste déroulante **Actions**.
4. Mettez à jour les **détails du certificat SSL** dans les zones de texte adéquates, puis cliquez sur **Mettre à jour** pour appliquer vos modifications. Pour plus d'informations, reportez-vous au tableau ci-dessous. 

   Les détails que vous entrez dans la fenêtre **Importer le certificat SSL** doivent reproduire fidèlement (espaces et sauts de ligne compris) les données qui vous ont été communiquées par l'autorité de certification. Dans le cas contraire, une erreur se produira.
   {:note}

| Détails d'un certificat SSL | Description |
| --------------------------- | ----------- |
|Certificat                  | Détails du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Clé privée                  | Détails de la clé privée du certificat fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Certificat intermédiaire    | Détails du certificat intermédiaire fournis par l'autorité de certification. Les certificats intermédiaires ne sont pas requis. Cependant, si les informations sont disponibles pour le certificat SSL, elles doivent être entrées.|
|Demande de signature de certificat | Détails de la demande de signature de certificat (CSR) fournis par l'autorité de certification. Ces détails ne sont pas requis, mais ils doivent être fournis s'ils font partie du certificat. **Remarque :** La demande de signature de certificat ne doit être changée en aucune manière. Une clé publique peut être incluse avec la demande. Elle ne doit pas être remplacée par la clé privée. |
|Remarques                        | Toutes notes concernant le certificat SSL qui peuvent être utiles aux autres utilisateurs.|
{: caption="Tableau 1. Détails d'un certificat SSL" caption-side="top"}

## Etapes suivantes

Une fois les détails du certificat SSL mis à jour, les produits ou services qui utilisaient déjà ce certificat ne sont pas impactés négativement par
les changements. Vous pouvez à tout moment effectuer une nouvelle mise à jour du certificat en répétant la procédure ci-dessus.
