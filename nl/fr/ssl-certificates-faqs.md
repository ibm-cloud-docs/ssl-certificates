---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Foire aux questions : certificats SSL

## Pourquoi le certificat SSL que j'ai commandé n'apparaît-il pas automatiquement sur l'écran des certificats SSL ?

Les certificats SSL sont délivrés par une autorité de certification tierce, qui
vous envoie tous les détails du certificat directement dans un e-mail confidentiel.
Après avoir reçu cet e-mail, vous avez la possibilité d'[importer le certificat SSL](import-ssl-certificate.html) sur le
portail {{site.data.keyword.slportal_full}}
si vous choisissez d'utiliser le certificat avec les produits et services {{site.data.keyword.BluSoftlayer_full}}.
Comme nous ne recevons jamais les détails du certificat SSL, nous ne pouvons pas importer ces données automatiquement.


## Qu'est-ce qu'un certificat SSL ?

Les certificats SSL sont utilisés par les sites web comme mesure de sécurité pour
protéger l'utilisateur final.
Ils sont généralement utilisés lorsqu'il vous est demandé de transmettre des informations
confidentielles à un site web, telles que vos nom, adresse, numéros de carte de crédit et
autres données personnelles, ou quand vous gérez des données qui nécessitent une
authentification (comme dans notre portail {{site.data.keyword.slportal}}).
Les certificats SSL sont demandés par la société qui exploite le site web, mais ils sont
délivrés par une société tierce de confiance qui garantit la validité du site web.
Les sites web sécurisés se reconnaissent à la chaîne HTTPS qui précède leur URL,
contrairement aux sites standard dont l'URL est précédée de HTTP.


## Comment puis-je commander un certificat SSL SHA2 ?

Si vous avez déjà commandé un certificat SSL et que des erreurs s'affichent,
indiquant que le certificat SSL utilise SHA-1 au lieu de SHA-2, vous devrez nous demander
de réémettre le certificat SSL.
Vous pouvez à cet effet soumettre un ticket.


Si vous n'avez pas encore commandé de certificat SSL chez nous et que vous avez besoin d'en
commander un qui utilise SHA-2, veuillez soumettre un ticket afin de commander manuellement un certificat SSL
pour le domaine concerné.
Les certificats SSL créés automatiquement par notre portail sont encore au niveau SHA-1. Par conséquent, si vous faites cela,
vous obtiendrez un certificat SHA-1 et vous devrez alors le faire réémettre.

