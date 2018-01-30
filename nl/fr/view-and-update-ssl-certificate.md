---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualisation et mise à jour des certificats SSL

Une fois qu'un certificat SSL a été importé dans l'écran Certificats SSL, vous
pouvez le voir et le mettre à jour à tout moment.
Les mises à jour fonctionnent de manière similaire au [processus d'importation](import-ssl-certificate.html). Tous les
détails mis à jour doivent correspondre exactement au certificat d'origine, y compris les espaces et les sauts de ligne.


Pour voir et mettre à jour un certificat SSL, effectuez les étapes suivantes.


1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
2. Sélectionnez **Afficher/mettre à jour le certificat** dans la
liste déroulante **Actions**.

3. Mettez à jour les **détails du certificat SSL** dans les zones de texte adéquates.


   **Remarque :** les détails que vous entrez dans la fenêtre **Importer le certificat SSL** doivent reproduire fidèlement
(espaces et sauts de ligne compris) les données qui vous ont été communiquées par l'autorité de certification.
Dans le cas contraire, une erreur se produira.


| Zone de texte | Entrée |
| -------- | ----- |
|Certificat |Détails du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Clé privée | Détails de la clé privée du certificat SSL fournis par l'autorité de certification. Il s'agit généralement d'un bloc de texte alphanumérique.|
|Certificat intermédiaire | Détails du certificat intermédiaire fournis par l'autorité de certification. Les certificats intermédiaires ne sont pas requis. Cependant, si les informations sont disponibles pour le certificat SSL, elles doivent être entrées.|
| Demande de signature de certificat | Détails de la demande de signature de certificat (CSR) fournis par l'autorité de certification. Ces détails ne sont pas requis, mais ils doivent être fournis s'ils font partie du certificat. **Remarque :** La demande de signature de certificat ne doit être changée en aucune manière. Une clé publique peut être incluse avec la demande. Elle ne doit pas être remplacée par la clé privée.|
|Remarques | Toutes notes concernant le certificat SSL qui peuvent être utiles aux autres utilisateurs.
Cliquez sur **Mettre à jour** pour mettre à jour le certificat SSL ou sur **Annuler** pour annuler l'opération.

## Etapes suivantes

Une fois les détails du certificat SSL mis à jour, les produits ou services qui utilisaient déjà ce certificat ne sont pas impactés négativement par
les changements.
Vous pouvez à tout moment effectuer une nouvelle mise à jour du certificat en répétant les étapes ci-dessus.

