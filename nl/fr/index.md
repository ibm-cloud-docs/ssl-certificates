---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Tutoriel Initiation
{: #getting-started-tutorial}

## Avant de commencer

Pour démarrer avec SSL, il faut un peu de planification. Effectuez les opérations prérequises suivantes.

1. Décidez où vous procurer le certificat
2. Renseignez-vous sur les types de certificats, la longueur des clés et leur
durée de validité
3. Choisissez un nom commun (ou nom usuel)
4. Découvrez la règle du socket
5. Générez la demande de signature de certificat

Pour plus d'informations, consultez [Planification SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## Commander les certificats SSL

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **Sécurité > SSL > Certificats**.
3. Sélectionnez **Commander le certificat SSL**. 
3. Sélectionnez le type et la durée du certificat, soumettez le texte de la demande de signature de certificat, sélectionnez votre plateforme de serveur et confirmez le paiement. 

## Installer et tester
Une fois le processus de commande et de validation terminé, vous recevez un e-mail de l'autorité de certification qui inclut votre certificat ainsi que les éventuels certificats intermédiaires nécessaires. La méthode d'installation dépend du logiciel que vous utilisez, mais le résultat devrait être le même. Une fois l'opération terminée, vous devez être en mesure d'accéder à `http://host.yourdomain.com` et de voir votre contenu, accompagné du cadenas SSL que les navigateurs utilisent pour indiquer une session cryptée. Si vous recevez un avertissement, il y a des mesures à prendre.

## Etapes suivantes

Une fois les tests réussis, vous pouvez accéder à vos certificats SSL dans la console {{site.data.keyword.cloud_notm}} pour [mettre à jour](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [télécharger](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [supprimer](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) ou [importer](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) des certificats SSL existants dans l'outil. 
