---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renouveler des certificats SSL
{: #renewing-ssl-certificates}

Une fois qu'un certificat SSL a été commandé via {{site.data.keyword.BluSoftlayer_full}}, il est possible de le renouveler à tout moment. {{site.data.keyword.BluSoftlayer_notm}} agit en tant que facilitateur entre le client (vous) et l'autorité de certification, et ne voit ni ne contrôle aucune partie du processus de renouvellement qui implique les détails du certificat SSL. Les certificats SSL sont renouvelés selon les mêmes termes que dans leur commande
précédente, de sorte qu'aucun changement ne peut être apporté aux détails du renouvellement (type de certificat et autorité de certification, mois de validité, plateforme serveur, etc.). Un certificat peut être renouvelé avant ou après son expiration. Cependant, pour qu'un certificat SSL soit valide sans interruption, pensez à le renouvelez avant sa date d'expiration. Pour renouveler un certificat SSL, procédez comme indiqué ci-après.

## Renouveler un certificat SSL

1. Accédez au portail [{{site.data.keyword.slportal_full}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window} en utilisant vos données d'identification uniques.
2. Dans le menu **Sécurité**, sélectionnez **SSL > Commandes**.
3. Cliquez sur le lien **Renouveler** dans la colonne **Renouveler**, sur la ligne du certificat SSL voulu.

   **Remarque :** une fenêtre apparaîtra pour vous permettre de compléter votre demande.  
   * Déterminez si tous les détails du renouvellement et de la demande de signature de certificat sont corrects :<br /><br /><table border="1"><caption>Tableau 1. Détails du renouvellement et de la demande de signature de certificat</caption><tr><th>Si...</th><th>Alors...</th></tr><tr><td>Tous les détails du renouvellement et de la demande de signature de certificat sont corrects</td><td>Passez à l'étape suivante.</td></tr><tr><td>Les détails du renouvellement sont incorrects</td><td><ul><li>Cliquez sur le lien <strong>achetez un nouveau certificat SSL</strong> pour être redirigé
vers l'écran d'achat.<br /><blockquote><strong>Remarque :</strong> étant donné qu'il n'est pas possible de changer les détails d'un certificat renouvelé,
en particulier son type, l'autorité de certification et l'adresse e-mail du valideur, le seul moyen de
changer les détails du certificat SSL d'un site web est de commander un nouveau certificat.</blockquote></li><li>Complétez les écrans de la page Commande avec les informations souhaitées pour le certificat SSL. Aucune autre action de cette procédure n'est nécessaire (puisque vous n'êtes plus dans le cas d'un renouvellement).</li></ul></td></tr><tr><td>Les détails de la demande de signature de certificat sont incorrects</td><td><ul><li>Cliquez sur le
bouton **Modifier demande de signature de certificat**.</li><li>Entrez les **nouveaux détails de la demande de signature de certificat** dans la
zone de texte **CSR**.</li><li>Cliquez sur le bouton **Restaurer demande de signature de certificat**.</li></ul></td></tr></table>
4. Cliquez sur le bouton **Renouveler** pour renouveler le certificat SSL ou sur **Annuler** pour annuler l'opération.

## Etapes suivantes

Une fois que vous avez demandé le renouvellement d'un certificat SSL, {{site.data.keyword.BluSoftlayer_notm}} transfère votre demande à l'autorité de certification afin qu'elle effectue les vérifications du site Web nécessaires au renouvellement. Une fois le certificat renouvelé, sa nouvelle date d'expiration s'affiche dans la zone correspondante.
