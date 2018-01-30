---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gérer les certificats SSL

{{site.data.keyword.BluSoftlayer_full}} offre à présent un moyen de stocker
les certificats dans son portail.
Non seulement cela peut servir de référentiel pour la gestion de vos certificats, mais c'est aussi une nécessité en cas
d'utilisation de services qui peuvent utiliser ou exiger des certificats.


1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats > Gérer les certificats**.

Une liste de vos certificats actuels vous est présentée accompagnée d'informations sur leur statut.


Vous pouvez rechercher des certificats, les télécharger en partie ou en totalité sous forme de fichiers PEM ou passer en revue leur date d'expiration.
Vous pouvez également voir combien de services utilisent actuellement chaque certificat.
Vous savez ainsi si des mesures doivent être prises lorsqu'un certificat est proche de son expiration.


## Ajouter un certificat

Lorsque vous êtes prêt à ajouter un certificat, sélectionnez l'option correspondante dans le sous-menu de navigation ou dans la
liste de certificats.
Vous n'êtes tenu de fournir que le certificat et sa clé privée.
En revanche, le fait de ne pas fournir de certificat intermédiaire alors que l'émetteur en fournit un peut rompre la chaîne de certificats et rendre incorrecte
la validation des utilisateurs finaux ou des services associés.


Remarque : les clés privées dont l'accès est protégé par une phrase de passe ne peuvent pas être stockées.

Une fois le ou les certificats ajoutés, les champs suivants sont dérivés directement :


* Nom commun
* Nom de l'organisation
* Période de validité


Et voilà ! 

## Editer un certificat

En activant le triangle à gauche d'un certificat, vous rendez ses différentes parties entièrement visibles.
Cela vous permet aussi de les éditer.
Vous pouvez ajouter une note au certificat et, en cas de nécessité, supprimer celui-ci.
Les services qui utilisent actuellement le certificat sont également listés.




Remarque importante : la mise à jour des parties "clé privée", "certificat" et "certificat intermédiaire" n'est pas possible pour les certificats associés à
des services.
Il n'est pas non plus possible de supprimer ces certificats.

La note jointe peut être modifiée à tout moment.


## Supprimer un certificat

Pour retirer un certificat, procédez comme pour l'éditer et cochez simplement la case "Confirm certificate removal" (confirmer le retrait ou la suppression du certificat) et sauvegardez.

### API

La possibilité d'ajouter, de retirer, d'éditer et de rechercher vos certificats est également disponible via la
SLAPI sldn.softlayer.com.
Certains exemples sont fournis dans l'article SLDN sldn.softlayer.com/article/SSL-Management-my-SLAPI-Its-more-likely-you-think.
