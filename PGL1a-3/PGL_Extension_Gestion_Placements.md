# Extension : gestion des placements

# Application cliente

## Compte-titres et profil d'investisseur

- Souscrire à un compte titre
  - En tant que client, je veux pouvoir demander l'ouverture d'un compte-titres afin d'acheter et de gérer des placements.
  ### Critères d'acceptation :
  - Le client doit posséder un portefeuille dans l'institution financière concernée.
  - Le client doit avoir un compte courant dans cette même institution.
  - Le client doit remplir le formulaire de profil d'investisseur.

- Remplir formulaire profil investisseur
  - En tant que client, je veux pouvoir remplir un formulaire afin que la banque détermine mon profil d'investisseur.
  ### Critères d'acceptation :
  - Le client doit demander l'ouverture d'un compte-titres ou vouloir modifier son profil actuel.

- Modifier profil investisseur
  - En tant que client, je veux pouvoir modifier mon profil d'investisseur afin qu'il corresponde à ma situation actuelle.
  ### Critères d'acceptation :
  - Le client doit déjà posséder un compte-titres et un profil d'investisseur.
  - Le client doit remplir à nouveau le formulaire.

## Consultation et gestion des investissements

- Gérer investissements
  - En tant que client, je veux pouvoir gérer mes investissements afin d'acheter ou de vendre des placements et de modifier mon profil.
  ### Critères d'acceptation :
  - Le portefeuille sélectionné doit contenir un compte-titres.

- Voir placements disponibles
  - En tant que client, je veux pouvoir voir les placements disponibles et leur historique afin de choisir ceux qui m'intéressent.
  ### Critères d'acceptation :
  - Le client doit posséder un compte-titres et un profil d'investisseur validé.
  - Les placements affichés doivent être compatibles avec son profil et la devise de son compte-titres.
  - Le client peut consulter l'historique d'un placement même s'il ne le possède pas.

- Filtrer placements en fonction du profil
  - En tant que client, je veux que les placements soient filtrés selon mon profil afin de voir ceux que je peux acheter.
  ### Critères d'acceptation :
  - Le client doit avoir un profil d'investisseur validé par la banque.
  - Les placements qui ne correspondent pas à son profil ne doivent pas être proposés à l'achat.

- Acheter placements
  - En tant que client, je veux pouvoir acheter des placements afin de les ajouter à mon compte-titres.
  ### Critères d'acceptation :
  - Le client doit posséder un compte-titres et un profil d'investisseur validé.
  - Le placement doit correspondre à son profil et à la devise du compte-titres.
  - Le client doit avoir assez d'argent pour payer l'achat et les frais.

- Vendre placements
  - En tant que client, je veux pouvoir vendre mes placements afin de récupérer mon argent.
  ### Critères d'acceptation :
  - Le client doit posséder le placement qu'il veut vendre.
  - La quantité à vendre doit être supérieure à zéro et ne peut pas dépasser la quantité détenue.
  - L'argent de la vente doit être versé sur un compte du client.

- Choix du compte courant pour réception d'argent
  - En tant que client, je veux pouvoir choisir le compte courant sur lequel recevoir l'argent de la vente d'un placement afin de décider où cet argent sera versé.
  ### Critères d'acceptation :
  - Le client doit être en train de vendre un placement.
  - Le client doit posséder au moins un compte courant pouvant recevoir l'argent.

## Visualisation et historique

- Visualiser placements
  - En tant que client, je veux pouvoir voir les placements de mon compte-titres afin de connaître leur valeur.
  ### Critères d'acceptation :
  - Le portefeuille sélectionné doit contenir un compte-titres.

- Visualiser historique des placements détenus
  - En tant que client, je veux pouvoir consulter l'historique de mes placements afin de voir leur évolution.
  ### Critères d'acceptation :
  - Le client doit posséder au moins un placement avec un historique disponible.

- Évolution de rendements et coûts de placements
  - En tant que client, je veux pouvoir voir l'évolution des rendements et des frais de mes placements afin de savoir combien ils rapportent et coûtent.
  ### Critères d'acceptation :
  - Le client doit posséder au moins un placement.
  - Des données de rendement et de frais doivent être disponibles pour la période choisie.

- Exporter données des placements
  - En tant que client, je veux pouvoir exporter les données de mes placements afin de les conserver ou de les partager.
  ### Critères d'acceptation :
  - Le client doit avoir des données de placements à exporter.
  - L'exportation doit être possible en CSV et en JSON.

# Application bancaire

## Profil d'investisseur

- Traiter une demande de profil investisseur
  - En tant qu'institution financière, je veux pouvoir traiter le formulaire d'un client afin de déterminer son profil d'investisseur.
  ### Critères d'acceptation :
  - Un client de l'institution doit avoir envoyé un formulaire de profil d'investisseur.

- Donner un profil à l'utilisateur
  - En tant qu'institution financière, je veux pouvoir attribuer un profil d'investisseur à un client afin de définir les placements auxquels il a accès.
  ### Critères d'acceptation :
  - Le formulaire du client doit avoir été rempli et validé.
  - Le profil attribué doit être conservateur, défensif, neutre, dynamique ou agressif.
