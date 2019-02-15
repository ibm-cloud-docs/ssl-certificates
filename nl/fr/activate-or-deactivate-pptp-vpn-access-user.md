---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Activer ou désactiver l'accès VPN PPTP

Le VPN PPTP permet aux utilisateurs de bénéficier d'un tunnel d'accès sécurisé au réseau privé {{site.data.keyword.BluSoftlayer_full}} en utilisant un logiciel client spécialisé sur leur ordinateur de bureau ou un appareil dédié. L'accès PPTP est conçu pour les clients qui doivent connecter un bureau entier ou qui ne
peuvent pas utiliser la solution VPN SSL. Chaque client se voit attribuer une unique connexion PPTP. Il peut obtenir plus de connexions sans frais supplémentaires mais il faut pour cela que le support technique active un accès PPTP illimité. Pour activer ou désactiver un accès VPN PPTP pour un utilisateur, effectuez les étapes suivantes.

1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques en tant qu'administrateur.
2. Localisez l'utilisateur dont vous souhaitez modifier l'accès et déterminez son niveau d'accès actuel en consultant la colonne **Accès au VPN**.
3. Dans le menu **Actions**, sélectionnez **Modifier accès au VPN**.
4. Entrez le type de VPN et les détails d'accès au sous-réseau.

|Nom de ma zone  |Options   |
| -----------| ------------ |
| Type de VPN   | Aucun, SSL, PPTP ou les deux (SSL et PPTP) |
|Accès au sous-réseau | Auto ou Manuel |           
{: caption="Tableau 1. Détails du VPN et du sous-réseau" caption-side="top"}   
5. Cliquez sur **Sauvegarder** pour sauvegarder vos changements.

   **Remarque :** pour qu'un utilisateur puisse se connecter en utilisant PPTP, l'accès PPTP doit être activé.
