---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Supprimer des certificats SSL
{: #deleting-ssl-certificates}

Lorsque les détails d'un certificat SSL ont été importés dans la console {{site.data.keyword.cloud}}, il est possible de les supprimer à tout moment pour éviter que les données ne soient sauvegardées dans la console {{site.data.keyword.cloud_notm}}.

Pour supprimer un certificat SSL, effectuez les étapes suivantes.

1. Accédez au menu de sécurité de votre console. Pour plus d'informations, consultez la rubrique relative à [l'accès aux appareils](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices). 
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Dans le menu **Actions**, sélectionnez l'option **Supprimer** pour le
certificat voulu.
4. Cliquez sur **Oui** pour supprimer le certificat SSL. 

## Etapes suivantes

Une fois qu'un certificat SSL a été supprimé, tous les services qui y sont liés cessent d'utiliser ses informations. Le certificat n'apparaît plus dans l'écran Certificats SSL de la console {{site.data.keyword.cloud_notm}}. 

Mettez à jour tous les services qui utilisaient jusqu'à présent le certificat supprimé afin de les lier à un certificat SSL valide et qui soit associé au compte. 

Vous pouvez à tout moment ajouter à nouveau le certificat SSL à la console {{site.data.keyword.cloud_notm}} à l'aide du processus d'[importation](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates).
{:note}
