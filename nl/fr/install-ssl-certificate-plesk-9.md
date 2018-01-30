---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installer un certificat SSL dans Plesk 9

Pour ajouter un certificat SSL dans Plesk 9, effectuez les étapes suivantes.


1. Connectez-vous à Plesk et naviguez jusqu'au domaine sur lequel vous voulez installer le certificat.
2. Entrez dans la configuration du domaine cible.
3. Cliquez sur **SSL certificates**.
4. Cliquez sur **Add SSL certificate**.

   **Remarque :** si vous avez déjà un certificat SSL, omettez cette étape et allez directement à l'étape 8.

5.  Nommez le certificat.
Vous pouvez lui donner n'importe quel nom, mais il peut être utile de choisir un nom descriptif, comprenant un
horodatage.


   Dans le cas présent, nous utilisons un nom au format *AAAAMMJJRR*, où *RR*
est le numéro de révision (00, car il n'y a pas de révision pour le même jour).

6. Apportez les ajustements nécessaires à la demande SSL.
Ces informations seront incorporées dans le certificat SSL. Elles doivent être similaires aux informations d'enregistrement du domaine.


  L'adresse e-mail doit correspondre à l'une des adresses du domaine dont les informations ont été fournies par votre registraire de noms de domaine.


  **Important :** toute information fausse sera rejetée par votre autorité de certification SSL.
7. Retournez dans la configuration des certificats.
8. Vérifiez la demande CSR et la clé privée et sauvegardée cette dernière en lieu sûr.
  

  **Remarque :** Si un problème quelconque avec votre serveur devait vous contraindre à réentrer les détails du certificat, il
vous faudrait au minimum le certificat lui-même et sa clé privée.

9. Prenez la demande CSR et soumettez-la à l'autorité de certification de votre choix.
L'infrastructure {{site.data.keyword.cloud_notm}} n'est pas une autorité à même de délivrer des certificats SSL.

10. Après avoir reçu le certificat de votre autorité de certification, vous pouvez le coller dans la zone de texte prévue à cet effet.


   **Remarques :**
   * Si votre autorité de certification l'impose, il est possible que vous deviez coller son propre certificat dans la
zone de texte du certificat d'AC (souvent appelé CA Bundle).

   * Pour pouvoir utiliser un certificat, vous devez être en possession de celui-ci et de sa clé privée.

11. Retournez à la partie *<span style="text-decoration: underline">Web Hosting Settings</span>* de la configuration Domains.

12. Sélectionnez le certificat correspondant et cliquez sur **OK**.

Le nouveau certificat est à présent utilisé pour le domaine.
Si vous avez mis à jour le certificat, pour que la nouvelle version soit utilisée, il est possible que vous deviez fermer entièrement
votre navigateur.

