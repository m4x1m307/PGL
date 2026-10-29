# Extension : gestion des placements

# Application cliente

## Compte-titres et profil d'investisseur

- Souscrire à un compte titre
  - En tant que client d'une institution financière, je veux pouvoir demander l'ouverture d'un compte-titres, afin d'acheter et de gérer des placements financiers.
  ### Critères d'acceptation :
    - Le client possède un portefeuille lié à l'institution auprès de laquelle il veut ouvrir le compte-titres.
    - Un compte-titres doit être lié à un compte courant dont le client est titulaire dans la même institution financière.
    - La souscription nécessite de remplir un formulaire de profil d'investisseur, transmis pour validation à l'institution.

- Remplir formulaire profil investisseur
  - En tant que client souhaitant investir, je veux pouvoir remplir un questionnaire sur ma situation et mes préférences, afin que l'institution financière puisse déterminer mon profil d'investisseur.
  ### Critères d'acceptation :
    - Le formulaire est accessible lors de la souscription à un compte-titres et lors d'une modification ultérieure du profil.

- Modifier profil investisseur
  - En tant que titulaire d'un compte-titres, je veux pouvoir soumettre un nouveau questionnaire de profil d'investisseur, afin d'adapter mon profil à l'évolution de ma situation et de mes objectifs.
  ### Critères d'acceptation :
    - Le client possède déjà un compte-titres et un profil d'investisseur.

## Consultation et gestion des investissements

- Gérer investissements
  - En tant que titulaire d'un compte-titres, je veux pouvoir accéder aux actions de gestion de mes investissements, afin d'acheter, de vendre mes placements ou de réévaluer mon profil d'investisseur.
  ### Critères d'acceptation :
    - Dans "Modifier portefeuille", la gestion des investissements est proposée lorsque le portefeuille sélectionné contient un compte-titres.
    - Sans compte-titres dans ce portefeuille, l'option de gestion des investissements n'est pas accessible.
    - L'application lui propose les opérations d'achat et de vente de placements.
    - L'application lui permet aussi d'accéder à la procédure de modification de son profil d'investisseur.

- Voir placements disponibles
  - En tant que titulaire d'un compte-titres, je veux pouvoir voir les placements que je peux acheter et consulter leur historique même si je ne les détiens pas, afin d'évaluer les investissements envisageables.
  ### Critères d'acceptation :
    - La liste ne présente que les placements compatibles avec le profil d'investisseur attribué au client.
    - Les placements disponibles respectent la devise du compte-titres ou du compartiment multidevises sélectionné.
    - Pour chaque placement proposé, le client peut consulter au minimum son nom, son type et son code ISIN.

- Filtrer placements en fonction du profil
  - En tant que titulaire d'un compte-titres, je veux que les placements disponibles soient filtrés en fonction de mon profil d'investisseur, afin de ne voir comme accessibles que les investissements adaptés au risque qui m'est autorisé.
  ### Critères d'acceptation :
    - Le filtrage utilise le profil validé par l'institution financière.
    - Les placements incompatibles avec ce profil ne sont pas accessibles à l'achat.

- Acheter placements
  - En tant que titulaire d'un compte-titres, je veux pouvoir acheter un placement financier disponible, afin de l'ajouter à mes investissements.
  ### Critères d'acceptation :
    - Le client possède un compte-titres et un profil d'investisseur attribué par l'institution financière.
    - Le placement choisi est compatible avec son profil et avec la devise du compte-titres ou de son compartiment.
    - Le client doit disposer des fonds nécessaires à l'achat et aux frais associés.

- Vendre placements
  - En tant que titulaire d'un compte-titres, je veux pouvoir vendre un placement que je détiens, afin de récupérer l'argent de cette vente sur l'un de mes comptes.
  ### Critères d'acceptation :
    - Le placement à vendre est présent dans un compte-titres du client.
    - La quantité vendue est positive et ne dépasse pas la quantité détenue.
    - L'argent reçu après la vente est versé sur un compte appartenant au client.

- Choix du compte courant pour réception d'argent
  - En tant que client souhaitant vendre un placement, je veux pouvoir sélectionner un compte courant pour recevoir le produit de la vente, afin de décider où sera versé l'argent récupéré.
  ### Critères d'acceptation :
    - Le client doit être en train d'effectuer une vente de placements.
    - Le client doit posséder au moins un compte courant pouvant recevoir l'argent.

## Visualisation et historique

- Visualiser placements
  - En tant que titulaire d'un compte-titres, je veux pouvoir visualiser les placements que je détiens, afin de connaître la composition et la valeur de mes investissements.
  ### Critères d'acceptation :
   - Le portefeuille sélectionné doit contenir un compte-titres.

- Visualiser historique des placements détenus
  - En tant que titulaire d'un compte-titres, je veux pouvoir consulter les données historiques de mes placements, afin de suivre leur évolution dans le temps.
  ### Critères d'acceptation :
    - Le client doit détenir au moins un placement dont les données historiques sont disponibles.

- Évolution de rendements et coûts de placements
  - En tant que titulaire d'un compte-titres, je veux pouvoir suivre l'évolution du rendement et des coûts de mes placements, afin de comprendre leur performance et les frais associés.
  ### Critères d'acceptation :
    - Le client doit détenir au moins un placement.
    - Des données de rendement et de coûts doivent être disponibles pour la période consultée.


- Exporter données des placements
  - En tant que titulaire d'un compte-titres, je veux pouvoir exporter les données de placements que je visualise, afin de les conserver et de les analyser hors de l'application.
  ### Critères d'acceptation :
    - Des données de placements doivent être disponibles à l'exportation.


# Application bancaire

## Profil d'investisseur

- Traiter une demande de profil investisseur
  - En tant qu'institution financière, je veux pouvoir recevoir et examiner le questionnaire d'un client souhaitant investir, afin de valider les informations nécessaires à l'attribution de son profil d'investisseur.
  ### Critères d'acceptation :
    - Une demande de profil d'investisseur doit avoir été envoyée par l'un de ses clients.

- Donner un profil à l'utilisateur
  - En tant qu'institution financière, je veux pouvoir attribuer à un client un profil d'investisseur à partir de son questionnaire validé, afin de déterminer les placements financiers auxquels il peut accéder.
  ### Critères d'acceptation :
    - Le questionnaire du client doit avoir été rempli et validé.
    - Le profil attribué appartient à l'une des cinq catégories : conservateur, défensif, neutre, dynamique ou agressif.

