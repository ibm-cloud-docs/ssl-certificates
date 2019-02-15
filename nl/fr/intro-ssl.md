---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introduction à la technologie SSL

SSL (Secure Sockets Layer) est une technologie qui chiffre le trafic entre l'application client et le serveur d'applications. Ce chiffrement est réalisé avec un système de clé publique/clé privée utilisant un certificat SSL.

Le certificat SSL contient la clé publique du serveur, les dates pour lesquelles le certificat est valide, un nom d'hôte pour lequel le certificat est valide et une signature de l'autorité de certification qui l'a émis.

## Terminologie SSL

Les certificats SSL ont une terminologie unique. Vous pouvez rencontrer les termes suivants lorsque vous utilisez des certificats SSL :

**Taille en bits :** les clés de chiffrement sont mesurées par leur taille en bits. Par exemple, 512 bits, 1024 bits, 2048 bits. Généralement, une clé longue sera plus sûre, mais aussi plus lente à utiliser. Actuellement, la taille minimale des clés utilisées dans les certificats SSL est de 1024 bits, bien que les certificats à validation étendue requièrent une clé 2048 bits.

**Chaîne de certificats :** les certificats SSL sont rarement utilisés seuls. Dans la plupart des installations, vous traitez une chaîne de certificats. Par
exemple :

  Racine > intermédiaire1 > cert serveur.

  \> Intermédiaire2 > cert serveur2

Dans cet exemple, le certificat de votre serveur est signé par le certificat
intermédiaire, qui à son tour est signé par le certificat racine. Chaîner les certificats de cette façon peut rendre SSL plus sûr, car cela signifie que le
certificat racine n'est pas utilisé (et exposé aux risques) si souvent. Si intermédiaire1 était compromis, il y aurait un risque pour cert serveur, mais cert serveur2 serait sûr, car il ne fait pas partie de la même chaîne.

**Demande de signature de certificat :** également appelée demande CSR (Certificate Signing Request), il s'agit d'un document que vous générez sur le serveur et qui contient les informations que l'autorité de certification utilisera pour créer votre certificat proprement dit.

**Nom commun :** parfois appelé nom usuel, le nom commun (CN, Common Name) est le nom d'hôte pour lequel le certificat est valide (par exemple, www.domaine.com).  

*Remarque :* www.domaine.com, smtp.domaine.com et mail.domaine.com sont trois noms d'hôte totalement entièrement différents. Un même certificat SSL ne pourrait être valide pour les trois (excepté si vous utilisiez un certificat générique, mais ce type de certificat n'est pas proposé actuellement par {{site.data.keyword.cloud}}).

**Clé privée/clé publique :** SSL repose sur une technique appelée cryptographie à clé publique. Dans cette forme de cryptographie, vous avez
deux clés : une clé publique et une clé privée. La clé publique est distribuée largement. En revanche, personne ne voit votre clé privée. Les personnes veulent communiquer en toute sécurité avec vous chiffrent leur communication avec votre clé publique. La cryptographie à clé publique est basée sur l'assertion selon laquelle les bits chiffrés avec une clé publique donnée ne peuvent être déchiffrés qu'en utilisant la clé privée correspondante et inversement.

**Certificat racine :** les certificats racine SSL sont des certificats signés par eux-mêmes et présentés au monde par leurs autorités de certification respectives. Les certificats racine des autorités de certification sont déjà installés dans le magasin de certificats de votre navigateur Web. Votre navigateur fait confiance à ces certificats, qui forment chacun le début d'une
chaîne de confiance menant au certificat que vous installez sur votre serveur.

**Signature :** les certificats SSL ont une signature numérique apposée par l'autorité de certification. C'est cette signature qui, tracée jusqu'au certificat racine de confiance, confirme
l'authenticité du certificat.

## SSL dans l'infrastructure IBM Cloud

{{site.data.keyword.BluSoftlayer_full}} revend trois types de certificats SSL : validation du domaine,
validation de l'organisation et validation étendue. 

Les certificats à validation du domaine (DV, Domain Validation) sont à la fois peu coûteux et
rapidement disponibles. La validation effectuée par l'autorité de certification se limite à l'envoi d'un e-mail à une adresse spécifiée sur le domaine concerné et à la réception d'une réponse positive. Les certificats à validation de l'organisation (OV, Organization Validation) et à validation étendue (EV, Extended Validation) s'obtiennent en quelques jours (parfois en une semaine), sont plus coûteux et entraînent des contrôles plus approfondis de la part de l'autorité de certification. Les certificats EV sont codés de telle manière que les navigateurs les reconnaissent comme tels et affichent une barre verte dans la barre d'adresse. 

Les certificats SSL, comme les autres services {{site.data.keyword.cloud_notm}}, peuvent être
gérés via le portail {{site.data.keyword.slportal}}. Accédez au menu **Sécurité** et sélectionnez l'option **Certificats SSL** pour commander et gérer vos certificats.  

**Remarque :** les certificats SSL commandés via {{site.data.keyword.cloud_notm}} ne doivent pas nécessairement être utilisés sur un serveur {{site.data.keyword.BluSoftlayer_notm}}. Réciproquement, les certificats commandés ailleurs sont utilisables sur vos serveurs hébergés ici.

Les certificats SSL améliorent la sécurité des transactions et donnent à vos utilisateurs un sentiment de sécurité. Parallèlement aux certificats SSL, la sécurité du démon (Daemon security), la sécurité
physique, les pratiques de codage et la gestion des certificats se combinent pour former
le profil de sécurité global de la solution.
