---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Planification SSL

Pour démarrer avec SSL, il faut un peu de planification.
Effectuez les opérations prérequises suivantes.

1. Décidez où vous procurer le certificat
2. Renseignez-vous sur les types de certificats, la longueur des clés et leur
durée de validité
3. Choisissez un nom commun (ou nom usuel)
4. Découvrez la règle du socket
5. Générez la demande de signature de certificat

## Décidez où vous procurer le certificat

Les certificats SSL peuvent être obtenus en interne dans votre organisation ou
auprès d'une autorité de certification, comme Verisign, RapidSSL, Thawte ou autre.
  

Dans une architecture contrôlée, pour un petit groupe tel que les employés d'une société
utilisant un site intranet, il est possible d'obtenir un certificat autosigné que chaque
employé installe ensuite dans son navigateur.
Vous pouvez également mettre en place votre propre autorité de certification locale afin
de générer des certificats utilisables dans votre organisation.


Pour un plus grand groupe, plus diversifié, l'utilisation d'un certificat SSL issu
d'une source standard permet un accès sans configuration spécialisée.
Les navigateurs web modernes sont configurés pour faire confiance aux certificats SSL
émis par les autorités de certification.


## Renseignez-vous sur les types de certificats, la longueur des clés et leur
durée de validité

Une fois que vous avez décidé où obtenir votre certificat, examinez les options
suivantes concernant les types de certificats et leur disponibilité, leur longueur de clé
et leur durée de validité.


|              Types de certificats       |  Disponibilité                    |  Longueur de clé           |  Durée                     |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Validation du domaine (DV)               | Rapidement disponible             | 1024 bits ou 2048 bits     | 1 ou 2 ans                 |
|Validation de l'organisation (OV)        | 2 à 3 jours, voire une semaine    | 1024 bits ou 2048 bits     | 1 ou 2 ans                 |
|Validation étendue (EV)                  | 2 à 3 jours, voire une semaine    | 2048 bits uniquement       | 1 ou 2 ans                 |
{: caption="Tableau 1. Types de certificats" caption-side="top"}   


## Choisissez un nom commun (ou nom usuel)

Le nom commun utilisé dans le certificat est le nom d'hôte du site web.
Le nom d'hôte et le nom commun du certificat doivent être identiques, sinon les navigateurs afficheront un avertissement.
Si votre site est web1.mondomaine.com, alors faites-en votre nom commun.
Si vous utilisez également images.mondomaine.com, vous devez soit utiliser
un certificat générique (non disponible auprès de {{site.data.keyword.cloud}}), soit configurer plusieurs
certificats.
Si vous choisissez le mauvais nom commun, des mesures peuvent être prises pour
corriger la commande de certificat ou pour révoquer le certificat obtenu et réémettre une demande avec
le nom commun adéquat.
  

## Découvrez la règle du socket

La limite est d'un certificat par socket.
Un socket est la combinaison d'une adresse IP et d'un port, telle que 1.2.3.4:443.
Comparée à l'exemple précédent, la combinaison 1.2.3.4:444 formerait un socket différent.
Pour les applications telles que SMTP/POP3 ou FTP, cela n'a pas d'importance.
Pour HTTP, en revanche, la notion de socket devient importante en raison de son rôle dans l'hébergement virtuel.


L'hébergement virtuel est la méthode par laquelle il est possible d'héberger 20, 30 ou même 100 sites sur une même
adresse IP.
Il tire parti d'une caractéristique particulière des navigateurs modernes, qui est celle de passer dans leur demande un champ appelé
en-tête d'hôte.
Ce champ, qui ressemble à quelque chose comme “Host: web1.mondomaine.com”, indique au serveur web à quel site
vous tentez d'accéder.
Dans le cas de HTTPS (HTTP sur SSL), le serveur web doit sélectionner le certificat SSL
à envoyer au client avant de voir l'en-tête d'hôte. C'est la raison pour laquelle un socket donné
ne peut avoir qu'un seul certificat.


Vous pouvez affecter chaque site web accessible sur SSL à son propre socket.
Il suffit, pour cela, de faire varier l'adresse IP ou le numéro de port.
Notez cependant que si vous utilisez autre chose que le port TCP standard 443,
les utilisateurs devront inclure explicitement le numéro de port dans l'URL (par exemple, https://web1.mondomaine.com:444).

## Générez la demande de signature de certificat

Vous pouvez générer la demande de signature de certificat en utilisant un logiciel sur le serveur web.
Pour les systèmes UNIX, utilisez le package OpenSSL.
Pour Windows, un assistant est accessible à partir de l'onglet Sécurité du répertoire des
propriétés du site web, dans Gestionnaire des services Internet (IIS).
Si vous utilisez un panneau de contrôle,
reportez-vous aux informations spécifiques de ce panneau.

La génération de la demande de signature de certificat s'accompagnera de la
création d'une clé privée.
Veillez à ne pas la perdre ni à la supprimer ou à la partager.
Elle doit rester privée sur le serveur web.
Certains utilitaires de génération de demande de signature de certificat offrent aussi la possibilité de créer une
phrase de passe pour protéger l'accès à la clé privée.
Ne faites pas cela, sauf si vous prévoyez de vous connecter au serveur à chaque
redémarrage du logiciel du serveur web.
Veillez en outre à ne pas appliquer d'expression de demande d'accès (challenge phrase) à la demande de signature de certificat.


