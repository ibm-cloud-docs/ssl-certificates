---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Supprimer des certificats SSL
{: #deleting-ssl-certificates}

Lorsque les détails d'un certificat SSL ont été importés dans le portail {{site.data.keyword.slportal_full}}, il est possible de les supprimer à tout moment pour éviter que les données ne soient sauvegardées sur le portail {{site.data.keyword.slportal}}.

Pour supprimer un certificat SSL, effectuez les étapes suivantes.

1. Accédez au portail [{{site.data.keyword.slportal}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Certificats**.
3. Dans le menu **Actions**, sélectionnez l'option **Supprimer** pour le
certificat voulu.

  **Remarque :** une fenêtre apparaît pour vous permettre de confirmer la suppression.
4. Cliquez sur **Oui** pour supprimer le certificat SSL ou sur **Non** pour annuler l'opération.

## Etapes suivantes

Une fois qu'un certificat SSL a été supprimé, tous les services qui y sont liés cessent d'utiliser ses informations. Le certificat n'certificat plus dans l'écran Certificats SSL du portail {{site.data.keyword.slportal}}.

Il est conseillé de mettre à jour tous les services qui utilisaient jusqu'à présent
le certificat supprimé afin de les lier à un certificat SSL valide et qui soit associé au
compte.

**Remarque :** vous pouvez à tout moment ajouter à nouveau le certificat SSL au portail {{site.data.keyword.slportal}} en utilisant le processus d'[importation](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates).
