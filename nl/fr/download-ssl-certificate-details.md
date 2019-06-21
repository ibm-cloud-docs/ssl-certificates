---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Télécharger les détails d'un certificat SSL
{: #downloading-ssl-certificate-details}

Une fois qu'un certificat SSL a été ajouté à la console {{site.data.keyword.cloud}}, ses détails peuvent être téléchargés à tout moment. Le téléchargement peut inclure le certificat seul, la clé seule ou le fichier PEM, qui comprend tous les détails disponibles sur le certificat SSL. Le téléchargement est sécurisé. Récupérer les détails par cette méthode est donc sans risque.
{:shortdesc}

Pour télécharger les détails d'un certificat SSL, effectuez les étapes suivantes.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Dans le menu **Actions**, sélectionnez l'**option de téléchargement** préférée pour le certificat. Pour plus d'informations, voir le tableau ci-dessous :

| Option de téléchargement | Informations de téléchargement |
| -------------------- | -------------------- |
| Télécharger le certificat | Limite le téléchargement à la partie certificat, en excluant la clé privée, le certificat intermédiaire, la demande de signature et les notes. |
| Télécharger la clé        | Limite le téléchargement à la clé privée, en excluant la partie certificat, le certificat intermédiaire, la demande de signature et les notes. |
| Télécharger PEM         | Télécharge tous les détails associés au certificat SSL, à savoir, la partie certificat, la clé privée, le certificat intermédiaire, la demande de signature et les notes. |
{: caption="Tableau 1. Options de téléchargement" caption-side="top"}

## Etapes suivantes

Lorsque vous demandez à télécharger les détails d'un certificat SSL, les
informations correspondantes sont automatiquement téléchargées dans le navigateur web. Sélectionnez le téléchargement pour ouvrir le fichier. Vous pouvez aussi sauvegarder le fichier sur votre poste de travail afin de pouvoir vous y référer ultérieurement. Vous pourrez à tout moment télécharger automatiquement les données de tout certificat présent sur l'écran Certificats SSL en répétant les étapes ci-dessus.

