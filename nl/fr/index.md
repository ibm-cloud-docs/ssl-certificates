---
copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Tutoriel Initiation  


## Avant de commencer

Pour démarrer avec SSL, il faut un peu de planification. Effectuez les opérations prérequises suivantes.

1. Décidez où vous procurer le certificat
2. Renseignez-vous sur les types de certificats, la longueur des clés et leur
durée de validité
3. Choisissez un nom commun (ou nom usuel)
4. Découvrez la règle du socket
5. Générez la demande de signature de certificat

Pour plus d'informations, consultez [Planification SSL](planning-ahead-ssl.html).

## Commander les certificats SSL

1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Sélectionnez **Sécurité > Certificats SSL>** pour accéder à l'écran
du même nom.
3. Vous devez sélectionner le type et la durée du certificat, soumettre le texte de la demande de signature de certificat, fournir quelques détails supplémentaires et confirmer le paiement.

## Installer et tester
Une fois le processus de commande et de validation terminé, vous recevez un e-mail de l'autorité de certification qui inclut votre certificat ainsi que les éventuels certificats intermédiaires nécessaires. La méthode d'installation dépend du logiciel que vous utilisez, mais le résultat devrait être le même. Une fois l'opération terminée, vous devez être en mesure d'accéder à <http://host.yourdomain.com> et de voir votre contenu, accompagné du cadenas SSL que les navigateurs utilisent pour indiquer une session cryptée. Si vous recevez un avertissement, il y a des mesures à prendre.

## Etapes suivantes

Une fois les tests réussis, vous pouvez accéder à l'écran des
certificats SSL pour [mettre à jour](view-and-update-ssl-certificate.html),
[télécharger](download-ssl-certificate-details.html), [supprimer](delete-ssl-certificate.html)
ou [importer](import-ssl-certificate.html) des certificats SSL existants dans l'outil.
