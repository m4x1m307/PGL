# Application cliente 
## Portefeuille
- Demander ajout d'un portefeuille
  - En tant que client,
  je veux pouvoir introduire une demande d'ouverture de portefeuille financier à une institution financière les détenant,
  afin de gérer les opérations concernant mes produits.
    #### Critères d'acceptation :
    - La demande de portefeuille est effectuée par un nouveau client     
    - Le client n'a pas encore de portefeuille dans l'application
    -  Le client détient au moins un produit financier dans une institution financière

- Modifier portefeuille
  - En tant que client d'une institution financière,
  je veux pouvoir modifier mon portefeuille,
  afin qu'il corresponde le mieux à mes besoins.
    #### Critères d'acceptations :
    - Le client a déjà fait une demande d'ajout de portefeuille et elle a été accepté par la banque
    - Le client a accès à son portefeuille

- Désactiver produits
	- En tant que client d'une institution financière,
	je veux pouvoir désactiver des produits financiers,
	afin de ne plus les voir car je ne veux pas les gérer.
	  #### Critères d'acceptation :
      - Le client possède un portefeuille avec au moins un produit financier dedans
	  - La désactivation (ainsi que le fait qu'il disparaisse) doit se faire immédiatement sans déconnexion
	  - Les produits désactivés doivent rester désactivés même après une deconnexion puis reconnexion 
  
- Réactiver produits
  - En tant que client d'une institution financière,
	je veux pouvoir réactiver les produits qui sont désactivés,
	afin de pouvoir les voir et le gérer.
	  #### Critères d'acceptation :
    - Le client doit avoir un portefeuille avec au moins un produit non-activé que j'avais sourscris auparavant 
    - La réactivation de ces produits vont se faire immédiatement
    - Les produits réactivés doivent le rester même si je me déconnecte
 
- Souscrire nouveaux produits
	- En tant que titulaire d'un portefeuille financier,
	je veux pouvoir souscrire à de nouveaux produits financiers.
	  #### Critères d'acceptation:
      - L'application doit informer le client qu'il a souscris à un nouveau produit quand il ouvre mon portefeuille
      - Les produits auquels il souscrit doivent être immédiatement disponible
      - Si un des produits pour lequel il a souscris est supprimer par l'institution financière, il doit être notifier quand il ouvre mon portefeuille

- Accéder au portefeuille
  - En tant que client connecté titulaire de produits financiers,
  je veux pouvoir visualiser mon portefeuille,
  afin de gérer mes produits.
    #### Critères d'acceptation : 
    - Le client doit être connecté à l'application 
    - Le client détient au moins un produit financier dans une institution financière
- Visualiser historique
  - En tant que client,
  je veux pouvoir visualiser l'historique de mes produits,
  afin de faire des opérations sur celles-ci.
    #### Critères d'acceptation : 
    - Le client doit avoir au moins un portefeuille
    - Le client doit être dans un portefeuille pour effectuer cette fonctionnalité 
    - Le client doit être connecté
    - Le client détient au moins un produit financier dans une institution financière
- Filtrer historique
  - En tant que client,
  je veux pouvoir filtrer l'historique selon une certaine période, certains produits financiers ou encore un ensemble de portefeuilles,
  afin de comparer les données dans le temps ou trouver certaines transactions.
    #### Critères d'acceptation : 
      - Le client détient au moins un portefeuille
      - Le client doit être connecté
      - Le client détient au moins un produit financier dans une institution financière
- Exporter données
    -  En tant que client,
    je veux pouvoir exporter l'historique au format CSV et JSON,
    afin de pouvoir l'imprimer ou le partager.
        #### Critères d'acceptation : 
       - Toute donnée filtrée est comprise dans l'historique uniquement
       - Le client détient au moins un portefeuille
       - Le client doit être connecté
       - Le client détient au moins un produit financier dans une institution financière
- Changer de type de visualisation
    - En tant que client,
    je veux pouvoir changer le format de la visualisation de mes produits (graphes, listes, tableaux,...).
      #### Critères d'acceptation : 
      - Le client détient au moins un portefeuille
      - Le client doit être connecté
      - Le client détient au moins un produit financier dans une institution financière
- Visualiser portefeuille
  - En tant que client,
  je veux pouvoir visualiser les produits financiers de mon portefeuille,
  afin de voir l'évolution des cours de ceux-ci.
    #### Critères d'acceptation : 
    - Le client détient au moins un portefeuille
    - Le client doit être connecté
    - Le client détient au moins un produit financier dans une institution financière
- Sélectionner produits à visualiser
  - En tant que client,
  je veux pouvoir sélectionner mes produits à visualiser,
  afin de comparer certains produits uniquement.
    #### Critères d'acceptation :
    - Les produits sélectionnés sont des produits appartenant au client
    - Le client doit être connecté
    - Le client détient au moins un produit financier dans une institution financière
- Changer de portefeuille 
  - En tan que client,
  je veux pouvoir changer de portefeuille,
  afin de voir mes différents produits dans diverses institutions.
    #### Critères d'acceptation : 
    - Le client détient au moins 1 portefeuille dans 2 institutions financières  
    - Le client doit être connecté
    - Le client doit déjà être dans un portefeuille durant cette action 
## Session
- Se connecter
  - En tant que client,
  je veux pouvoir me connecter à l'application client,
  afin d'avoir accès à mes données.
    #### Critères d'acceptation : 
     - Le client ne peut pas se connecter à 2 appareils différents simultanément
- Créer un compte
  - En tant qu'utilisateur,
  je veux pouvoir créer un compte,
  afin d'accéder à toutes les fonctionnalités que l'institution financière propose.
    #### Critères d'acceptation :
    - Lorsque le client créé un compte, l'application doit le retenir et il ne doit plus en recréer un lors de sa reconnexion
    - Le client n'a pas encore de compte créé dans l'application
- Choisir langue préférée
  - En tant qu'utilisateur venant de créer un compte,
  je veux choisir ma langue préférée et la mémoriser,
  afin d'avoir la meilleure expérience possible.
    #### Critères d'acceptation :
    - Le client ne doit pas resélectionner sa langue préférée quand il se reconnecte
    - L'application lui propose un champ pour indiquer sa langue
    - Une langue par défaut est déjà écrite dans le champ
- Exécution session
  - En tant que client,
  je veux pouvoir exécuter la session,
  afin de faire différentes actions sur l'application client.
     #### Critères d'acceptation :
    - Le client doit être connecté 
-  Réinitialiser mot de passe
    - En tant que client,
    je veux pouvoir réinitialiser mon mot de passe,
    afin de me protéger d'un futur oubli ou d'une fuite de données.
        #### Critères d'acceptation : 
      - Le client doit être connecté 
      - Le client doit connaître son mot de passe pour le changer
- Changer langue
  - En tant qu'utilisateur non-connécté,
  je veux pouvoir choisir la langue de la page d'acceuil,
  afin de suivre les instructions dans la langue de mon choix.
    #### Critères d'acceptation :
    - L'application lui propose un sélecteur de langue
    - L'application doit avoir toutes ses informations dans la langue qu'il a choisie
- Changer langue préférée
  - En tant qu'utilisateur déjà connecté,
  je veux pouvoir changer ma langue préférée plus tard,
  afin d'utiliser l'application avec la langue que je désire pour la connexion actuelle et les prochaines connexions.
    #### Critères d'acceptation :
    - Une option est disponible pour changer sa langue préférée
    - Le changement est immédiat, pas besoin de se déconnecter
    - Son nouveau choix est enregistrer et ne doit pas changer tant qu'il ne le change pas manuellement
- Fermer session
  - En tant qu'utilisateur,
  je veux pouvoir fermer la session en me déconnectant,
  afin de pouvoir me connecter sur un autre appareil ou quitter l'application.
    #### Critères d'acceptation :
    - Le client peut se reconnecter à tout moment à condition que personne ne soit connecté en même temps
    - L'application possède un bouton pour pouvoir se déconnecter
    - L'utilisateur est connecté avant de fermer la session 
## Virements
- Demande ajout de la fonctionnalité
	- En tant que titulaire d'un portefeuille,  
	je veux pouvoir faire une demande,  
	afin d'obtenir la fonctionnalité de virement.  
      #### Critères d'acceptation :
        - Une fois la demande accepté, l'application doit retenir que la demande du client a été accepter et ne dois pas lui enlever la fonctionnalité même lors de la déconnexion

- Effectuer un virement
	- En tant que titulaire d'un portefeuille,  
	je veux pouvoir effectuer un virement vers un autre compte,  
	afin de transférer de l'argent sans avoir besoin d'une carte bancaire.
	  #### Critères d'acceptation :
	    - Une demande pour obtenir la fonctionnalité a déjà été introduite et acceptée par la banque
      - Le client doit être dans un de ses portefeuille
- Sélectionner compte dans portefeuille
  - En tant qu'utilisateur possèdant un portefeuille,
  je veux pouvoir Sélectionner un compte dans mon portefeuille,
  afin d'effectuer un virement avec celui ci.
    #### Critères d'acceptation :
    - L'application nous montre tous les compte qu'on peut choisir pour effectuer un virement
- Préciser compte et nom du destinataire
  - En tant qu'utilisateur voulant effectuer un virement,
  je veux pouvoir spécifier compte et le nom du destinataire,
  afin que la personne que je désire reçoive bien le virement
    #### Critères d'acceptation :
    - Le nom du destinataire doit correspondre au nom du titulaire du compte de destination
- Choisir montant à transférer
  - En tant qu'utilisateur voulant effectuer un virement,
  je veux pouvoir choisir le montant pour le virement,
  afin que celui ci ne dépasse pas le solde de mon compte.
    #### Critères d'acceptation :
    - Le montant à virer doit être inférieur ou égal au montant sur le compte, mais aussi positif
# Application bancaire
## Session

- Exécuter session
  - En tant qu'institution financière, je veux pouvoir accéder aux différentes fonctionnalités de l'application afin de gérer mes clients et leurs produits financiers.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée à l'application.
- Se connecter
  - En tant qu'institution financière, je veux pouvoir me connecter à l'application afin de gérer mes clients et leurs produits financiers.
  #### Critères d'acceptation :
  - L'institution doit posséder un login et un mot de passe.
  - Le login et le mot de passe doivent être corrects.
- Changer MDP
  - En tant qu'institution financière, je veux pouvoir changer mon mot de passe afin de sécuriser mon compte.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
  - L'ancien mot de passe doit être correct.
- Fermer session
  - En tant qu'institution financière, je veux pouvoir me déconnecter de l'application afin de terminer ma session.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
- Traiter une demande
  - En tant qu'institution financière, je veux pouvoir traiter les demandes de mes clients afin de les accepter ou de les refuser.
  #### Critères d'acceptation :
  - L'application doit avoir reçu au moins une demande.
  - La demande doit concerner un client de l'institution financière.

## Clients

- Gérer clients
  - En tant qu'institution financière, je veux pouvoir gérer mes clients afin d'ajouter ou de supprimer des clients de mon institution.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée à l'application.
- Ajouter un client
  - En tant qu'institution financière, je veux pouvoir ajouter un nouveau client afin de lui proposer mes produits financiers.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
  - Les informations du nouveau client doivent être renseignées.
  - Le client ne doit pas déjà être enregistré dans cette institution.
- Supprimer un client
  - En tant qu'institution financière, je veux pouvoir supprimer un client afin qu'il ne fasse plus partie de mes clients.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
  - Le client doit déjà faire partie de l'institution financière.

## Virements

- Traiter une demande de fonctionnalité de virement
  - En tant qu'institution financière, je veux pouvoir traiter une demande de fonctionnalité de virement afin de permettre ou non à mes clients d'effectuer des virements.
  #### Critères d'acceptation :
  - L'application doit avoir reçu une demande de fonctionnalité de virement.
  - Le client doit posséder au moins un compte dans l'institution financière.
- Approuver une demande
  - En tant qu'institution financière, je veux pouvoir accepter une demande de fonctionnalité de virement afin que mon client puisse effectuer des virements.
  #### Critères d'acceptation :
  - Le client doit avoir effectué une demande au préalable.
  - Le client doit posséder au moins un compte dans l'institution financière.
- Refuser une demande
  - En tant qu'institution financière, je veux pouvoir refuser une demande de fonctionnalité de virement afin d'empêcher un client d'utiliser cette fonctionnalité.
  #### Critères d'acceptation :
  - Le client doit avoir effectué une demande au préalable.
  - La demande doit concerner l'institution financière connectée.

## Produits financiers

- Gérer produits financiers
  - En tant qu'institution financière, je veux pouvoir gérer les produits financiers de mes clients afin d'ouvrir ou de clôturer leurs produits.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
  - Les produits financiers doivent appartenir à son institution.
- Ouvrir un produit financier
  - En tant qu'institution financière, je veux pouvoir ouvrir un nouveau produit financier pour un client afin qu'il puisse l'utiliser.
  #### Critères d'acceptation :
  - Le client doit faire partie de l'institution financière.
  - Le produit financier doit être proposé par l'institution.
- Clôturer un produit financier
  - En tant qu'institution financière, je veux pouvoir clôturer un produit financier afin de mettre fin à son utilisation par un client.
  #### Critères d'acceptation :
  - Le produit financier doit être ouvert.
  - Le produit doit appartenir à un client de l'institution financière.
- Traiter une demande de gestion de produits
  - En tant qu'institution financière, je veux pouvoir traiter les demandes de gestion de produits de mes clients afin de répondre à leurs demandes d'ouverture ou de fermeture.
  #### Critères d'acceptation :
  - Le client doit avoir envoyé une demande au préalable.
  - La demande doit concerner un produit financier de l'institution.
- Traiter une demande d'ouverture
  - En tant qu'institution financière, je veux pouvoir traiter une demande d'ouverture de produit afin de permettre à un client de souscrire à un nouveau produit financier.
  #### Critères d'acceptation :
  - Le client doit avoir effectué une demande d'ouverture.
  - Le produit doit faire partie des produits proposés par l'institution financière.
  - Le client doit faire partie de l'institution financière.
- Traiter une demande de fermeture
  - En tant qu'institution financière, je veux pouvoir traiter une demande de fermeture de produit afin de permettre à un client de clôturer un produit financier.
  #### Critères d'acceptation :
  - Le client doit avoir effectué une demande de fermeture.
  - Le produit financier doit déjà être ouvert.
  - Le produit doit appartenir à un client de l'institution financière.

## Lister des données

- Lister les clients
  - En tant qu'institution financière, je veux pouvoir afficher la liste de mes clients afin de consulter leurs informations.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
- Lister les produits financiers liés à un client
  - En tant qu'institution financière, je veux pouvoir afficher les produits financiers d'un client afin de consulter les produits qu'il possède dans mon institution.
  #### Critères d'acceptation :
  - Le client doit faire partie de l'institution financière.
  - Seuls les produits financiers liés à cette institution doivent être affichés.
- Filtrer produits
  - En tant qu'institution financière, je veux pouvoir filtrer les produits financiers afin de trouver plus facilement les produits que je recherche.
  #### Critères d'acceptation :
  - L'institution financière doit être en train de consulter une liste de produits financiers.
  - L'application doit permettre de sélectionner un ou plusieurs critères de filtrage.

## Exportation et importation

- Exporter données
  - En tant qu'institution financière, je veux pouvoir exporter les données que je consulte afin de les imprimer ou de les partager ou de les analiser.
  #### Critères d'acceptation :
  - L'institution financière doit avoir des données à exporter.
  - L'application doit proposer les formats CSV et JSON.
- Importer fichiers de données
  - En tant qu'institution financière, je veux pouvoir importer des fichiers de données afin d'ajouter des informations dans la base de données.
  #### Critères d'acceptation :
  - L'institution financière doit être connectée.
  - Les fichiers doivent contenir uniquement des informations appartenant à l'institution financière connectée.
