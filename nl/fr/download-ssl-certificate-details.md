---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Télécharger les détails d'un certificat SSL

Une fois qu'un certificat SSL a été ajouté au portail {{site.data.keyword.slportal_full}}, ses détails peuvent être téléchargés à tout moment. Le téléchargement peut inclure le certificat seul, la clé seule ou le fichier PEM, qui comprend tous les détails disponibles sur le certificat SSL. Le téléchargement est sécurisé. Récupérer les détails par cette méthode est donc sans risque.

Pour télécharger les détails d'un certificat SSL, effectuez les étapes suivantes.

1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Dans le menu **Actions**, sélectionnez l'**option de téléchargement** préférée pour le certificat. Pour plus d'informations, voir le tableau ci-dessous :

| Option de téléchargement      | Informations de téléchargement |
| -------------------- | -------------------- |
| Télécharger le certificat | Limite le téléchargement à la partie certificat, en excluant la clé privée, le certificat intermédiaire, la demande de signature (CSR) et les Notes (ou Remarques). |
| Télécharger la clé         | Limite le téléchargement à la clé privée, en excluant la partie certificat, le certificat intermédiaire, la demande de signature (CSR) et les Notes (ou Remarques). |
| Télécharger PEM         | Télécharge tous les détails associés au certificat SSL, ce qui comprend la partie certificat, la clé privée, le certificat intermédiaire, la demande de signature (CSR) et les Notes (ou Remarques). |
{: caption="Tableau 1. Options de téléchargement" caption-side="top"}

## Etapes suivantes

Lorsque vous demandez à télécharger les détails d'un certificat SSL, les
informations correspondantes sont automatiquement téléchargées dans le navigateur web. Sélectionnez le téléchargement pour ouvrir le fichier. Vous pouvez aussi sauvegarder le fichier sur votre poste de travail afin de pouvoir vous y référer ultérieurement. Vous pourrez à tout moment télécharger automatiquement les données de tout certificat présent sur l'écran Certificats SSL en répétant les étapes ci-dessus.
