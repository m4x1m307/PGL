# Application cliente 
## Portefeuille
- Demander ajout d'un portefeuille
  - En tant que client,
  je pouvoir introduire une demande d'ouverture de portefeuille financier à une institution financière les détenant,
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
    - J'ai déjà fait une demande d'ajout de portefeuille et elle a été accepté par la banque
    - J'ai accès à mon portefeuille

- Désactiver produits
	- En tant que titulaire d'un portefeuille financier possédant des produits,
	je veux pouvoir désactiver des produits financiers,
	afin de ne plus les voir car je ne veux pas les gérer.
	  #### Critères d'acceptation :
	  - Je dois posséder au moins un produit financier
	  - La désactivation (ainsi que le fait qu'il disparaisse) doit se faire immédiatement sans déconnexion
	  - les produits désactivés doivent rester désactivés même après une deconnexion puis reconnexion 
  
- Réactiver produits
  - En tant que client possédant des produits financiers dans son portefeuille,
	je veux pouvoir réactiver les produits qui sont désactivés,
	afin de pouvoir les voir et le gérer.
	  #### Critères d'acceptation :
    - Je dois avoir au moins un produit non-activé
    - La réactivation de ces produits vont se faire immédiatement
    - Les produits réactivés doivent le rester même si je me déconnecte
 
- Souscrire nouveaux produits
	- En tant que titulaire d'un portefeuille financier,
	je veux pouvoir souscrire à de nouveaux produits financiers.
	  #### Critères d'acceptation:
      - L'application doit m'informer que j'ai souscris à un nouveau produit quand j'ouvre mon portefeuille
      - Les produits auquels je souscris doivent être immédiatement disponible
      - Si un des produits pour lequel j'ai souscris est supprimer par l'institution financière, je dois être notifier quand j'ouvre mon portefeuille

- Accéder au portefeuille
  - En tant que client connecté titulaire de produits financiers,
  je veux pouvoir visualiser mon portefeuille,
  afin de gérer mes produits.
    #### Critères d'acceptation : 
    - Le client doit être connecté à l'application 
    - Le client détient au moins un produit financier dans une institution financièr
- Visualiser historique
  - En tant que client connecté titulaire de produits financiers,
  je veux pouvoir visualiser l'historique de mes produits,
  afin de faire des opérations sur celles-ci.
    #### Critères d'acceptation : 
    - Le client doit avoir au moins un portefeuille 
    - Le client doit être connecté
- Filtrer historique
  - En tant que client connecté titulaire de produits financiers,
  je veux pouvoir filtrer l'historique selon une certaine période, certains produits financiers ou encore un ensemble de portefeuilles,
  afin de comparer les données dans le temps ou trouver certaines transactions.
    #### Critères d'acceptation : 
      - Le client détient au moins un portefeuille
      - Le client doit être connecté
- Exporter données
    -  En tant que client,
    je veux pouvoir exporter l'historique au format CSV,
    afin de pouvoir l'imprimer ou le partager.
        #### Critères d'acceptation : 
       - Toute donnée filtrée est comprise dans l'historique uniquement
       - Le client détient au moins un portefeuille
       - Le client doit être connecté
- Changer de type de visualisation
    - En tant que client,
    je veux pouvoir changer le format de la visualisation de mes produits (graphes, listes, tableaux,...).
      #### Critères d'acceptation : 
      - Le client détient au moins un portefeuille
      - Le client doit être connecté
- Visualiser portefeuille
  - En tant que client,
  je veux pouvoir visualiser les produits financiers de mon portefeuille,
  afin de voir l'évolution des cours de ceux-ci.
    #### Critères d'acceptation : 
    - Le client détient au moins un portefeuille
    - Le client doit être connecté
- Sélectionner produits à visualiser
  - En tant que client,
  je veux pouvoir sélectionner mes produits à visualiser,
  afin de comparer certains produits uniquement.
    #### Critères d'acceptation :
    - Les produits sélectionnés sont des produits appartenant au client
    - Le client doit être connecté
- Changer de portefeuille 
  - En tan que client connecté titulaire de produits financiers dans diverses institutions,
  je veux pouvoir changer de portefeuille,
  afin de voir mes différents produits dans diverses institutions.
    #### Critères d'acceptation : 
    - Le client détient au moins 2 portefeuilles 
    - Le client doit être connecté
## Session
- Se connecter
  - En tant que client,
  je veux pouvoir me connecter à l'application client,
  afin d'avoir accès à mes données.
    #### Critères d'acceptation : 
     - Le client ne peut pas se connecter à 2 appareils différents simultanément
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
## Virements
- Demande ajout de la fonctionnalité
	- En tant que titulaire d'un portefeuille,  
	je veux pouvoir faire une demande,  
	afin d'obtenir la fonctionnalité de virement.  
      #### Critères d'acceptation :
        - Une fois la demande accepté, l'application doit retenir que ma demande a été accepter et ne dois pas m'enlever la fonctionnalité même lors de la déconnexion

- Effectuer un virement
	- En tant que titulaire d'un portefeuille,  
	je veux pouvoir effectuer un virement vers un autre compte,  
	afin de transférer de l'argent sans avoir besoin d'une carte bancaire.
	  #### Critères d'acceptation :
	    - Une demande pour obtenir la fonctionnalité a déjà été introduite et acceptée par la banque
	    - Le compte et le nom du destinataire doivent être spécifiés
	    - Le compte depuis lequel on veut virer cet argent doit être sélectionné
	    - Un montant à virer doit être précisé
	    - Le nom du destinataire doit correspondre au nom du titulaire du compte de destination 
	    - Le montant à virer doit être inférieur ou égal au montant sur le compte, mais aussi positif 

# Application bancaire
## Session
- Traiter une demande 
  - En tant qu'institution financière,
  je veux pouvoir regarder les identifiants dans une demande de portefeuille financier d'un nouveau client,
  afin de vérifier s'il est client de l'institution et poursuivre la procédure de réponse à cette demande.
    #### Critères d'acceptation : 
     - 1
     - 2

## Clients

## Virements
- Traiter demande de gestion de virement
  - En tant qu'institution financière,
  je veux pouvoir traiter une demande de gestion de virement,
  afin que mes clients puissent avoir accès (ou non) à la fonctionnalité.
    #### Critères d'acceptation :
    - L'application doit avoir reçue au moins une demande pour obtenir la fonctionnalité de la part d'un client
- Approuver une demande
  - En tant qu'institution financière,
  je veux pouvoir accepté une demande pour la fonctionnalité de virement pour des clients,
  afin qu'ils puissent effectuer des virements avec leurs comptes 
    #### Critères d'acceptation :
    - Le client doit posséder au moins un compte de l'institution financière pour laquelle il a fait une demande 
    - Le client doit avoir effectuer une demande au préalable
    - Une fois la demande acceptée pour un client, l'application doit retenir que le client en question a déjà fait une demande et qu'elle a été acceptée
- Refuser une demande
  - En tant qu'institution financière,
  je veux pouvoir refuser une demande pour la fonctionnalité de virement pour des clients,
  afin d'empêcher des clients qui ne sont pas considérés comme apte à avoir cette fonctionnalité, de l'obtenir
    #### Critères d'acceptation
    - Le client doit avoir effectuer une demande au préalable
## Produits financiers
- Traiter une demande de gestion de produits
  - En tant qu'institution financière,
  je veux pouvoir traiter une demande de gestion de produit introduite par un client,
  afin que celui ci puisse gérer ses produits comme bon lui semble.
    #### Critères d'acceptation :
    - Le client doit avoir envoyé une demande au préalable
- Traiter une demande d'ouverture
  - En tant qu'institution financière,
  je veux pouvoir traiter une demande d'ouverture de produit,
  afin que le client ayant fait la demande puisse ajouter un produit à son portefeuille.
    #### Critères d'acceptation :
    - Le client doit avoir fait cette demande spécifique au préalable
    - Le produit doit figurer parmi les produits que l'institution financière propose
- Traiter une demande de fermeture
  - En tant qu'institution financière,
  je veux pouvoir traiter une demande de fermeture de produit,
  afin de permettre à un client de ne plus vouloir gérer ce produit.
    #### Critères d'acceptation :
    - Le client doit avoir ce produit déjà ouvert dans son portefeuille au moment de la demande
