---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Activer ou désactiver l'accès VPN PPTP
{: #activating-or-deactivating-pptp-vpn-access}

Le VPN PPTP vous permet de bénéficier d'un tunnel d'accès sécurisé au réseau privé {{site.data.keyword.cloud}} en utilisant un logiciel client spécialisé sur votre ordinateur de bureau ou un appareil dédié. L'accès PPTP est conçu pour le cas où vous devez connecter un bureau entier ou ne pouvez pas utiliser la solution VPN SSL. Une unique connexion PPTP vous est attribuée. Vous pouvez obtenir plus de connexions sans frais supplémentaires mais il faut pour cela que le support technique active un accès PPTP illimité. Pour activer ou désactiver un accès VPN PPTP pour un utilisateur, effectuez les étapes suivantes.
{:shortdesc}

1. Connectez-vous à la page [Accès (IAM)](https://cloud.ibm.com/iam/overview){: external} de la console {{site.data.keyword.cloud_notm}}. 
2. Localisez l'utilisateur dont vous souhaitez modifier l'accès et déterminez son niveau d'accès actuel en consultant la colonne **Accès au VPN**.
3. Dans le menu **Actions**, sélectionnez **Modifier accès au VPN**.
4. Entrez le type de VPN et les détails d'accès au sous-réseau, puis cliquez sur **Sauvegarder** pour sauvegarder vos changements. Pour plus d'informations, reportez-vous au tableau ci-dessous. 

|Nom de ma zone  |Options   |
| -----------| ------------ |
| Type de VPN   | Aucun, SSL, PPTP ou les deux (SSL et PPTP) |
| Accès au sous-réseau | Auto ou manuel |           
{: caption="Tableau 1. Détails du VPN et du sous-réseau" caption-side="top"}   

Pour qu'un utilisateur puisse se connecter en utilisant PPTP, l'accès PPTP doit être activé.{:note}
