---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gérer les certificats SSL
{: #managing-ssl-certificates}

Vous pouvez gérer vos certificats SSL dans la console {{site.data.keyword.cloud}}. Non seulement cela peut servir de référentiel pour la gestion de vos certificats, mais c'est aussi une nécessité en cas
d'utilisation de services qui peuvent utiliser ou exiger des certificats.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats > Gérer les certificats**.


Une liste de vos certificats actuels vous est présentée accompagnée d'informations sur leur statut.

Vous pouvez rechercher des certificats, les télécharger en partie ou en totalité sous forme de fichiers PEM ou passer en revue leur date d'expiration. Vous pouvez également voir combien de services utilisent actuellement chaque certificat. Vous savez ainsi si des mesures doivent être prises lorsqu'un certificat est proche de son expiration.

## Ajouter un certificat

Lorsque vous êtes prêt à ajouter un certificat, sélectionnez **Ajouter un certificat** dans le sous-menu de navigation ou dans la liste de certificats. Vous n'êtes tenu de fournir que le certificat et sa clé privée. En revanche, le fait de ne pas fournir de certificat intermédiaire alors que l'émetteur en fournit un peut rompre la chaîne de certificats et rendre incorrecte la validation des utilisateurs ou des services associés.

Les clés privées dont l'accès est protégé par une phrase de passe ne peuvent pas être stockées. {:note}

Une fois le ou les certificats ajoutés, les zones suivantes sont dérivées directement :

* Nom usuel
* Nom de l'organisation
* Période de validité

## Editer un certificat

Lorsque vous activez le triangle à gauche d'un certificat, ses différentes parties s'affichent entièrement. Cela vous permet aussi de les éditer. Vous pouvez ajouter une note au certificat et, en cas de nécessité, supprimer celui-ci. Les services qui utilisent actuellement le certificat sont également listés.

La mise à jour des parties clé privée, certificat et certificat intermédiaire n'est pas possible pour les certificats associés à des services. Il n'est pas non plus possible de supprimer ces certificats. La note jointe peut être modifiée à tout moment.

## Supprimer un certificat

Pour supprimer un certificat, procédez comme pour l'éditer et cochez simplement la case "Confirm certificate removal", puis sauvegardez.

## Utilisation de l'API

Pour un exemple d'édition de certificats à l'aide de l'API, voir [Gestion SSL![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](http://sldn.softlayer.com/article/ssl-management){: new_window}.
