# Application cliente 
## Portefeuille
- Demander ajout d'un portefeuille
  - EN TANT QUE client, JE VEUX pouvoir introduire une demande d'ouverture de portefeuille financier à une institution financière les détenant AFIN de gérer les opérations concernant mes produits
    #### Critères d'acceptation :
    - La demande de portefeuille est effectuée par un nouveau client     
    - Le client n'a pas encore de portefeuille dans l'application
    -  Le client détient au moins un produit financier dans une institution financière
portefeuille financier = ensemble de produits financiers

Use cases :
	- Ajouter de nouveaux clients dans la BDD de l'institution financière 
	- Créer un portefeuille financier
	- Gérer 1 portefeuille financier
	- Gestion de l'ensemble des portefeuilles financiers d'1 client
	- Accès aux produits financiers (mdp + login)
	- Réinitialisation mdp 
	- Authentification/déconnection de l'application
	- 
	
User stories :

- Authentification 
	* 2 connexions différentes interdites en mm temps
	En tant qu'user connecté pour la 1e fois, 
		je veux pouvoir introduire une demande de création de portefeuille
	* 
	    En tant qu'user connecté, 
		je veux pouvoir me déconnecter
		je veux pouvoir changer mon mdp
		je ne veux pas qu'un autre appareil soit connecté en même tant
		que celui utilisé 
		
## Portefeuille 
- En tant que client connecté,
    		je veux pouvoir consulter mon portefeuille financier
    		je veux pouvoir désactiver/réactiver des produits 
    		de mon portefeuille
    		je veux pouvoir demander l'ouverture/fermeture d'un compte
    		je suis titulaire
    		je veux que les produits que je supprime soient archivés
    		je veux pouvoir souscrire à un produit 
    		
- En tant que client ouvrant mon portefeuille, 
    		je veux être averti lors d'une souscription à un nouveau produit
    		ou si l'institution décide de supprimer un produit dont je suis titulaire

	### Fonctionnalité de modification du portefeuille
	#### Désactivation de produits financiers:
	- En tant que titulaire d'un portefeuille financier possédant des produits,
	je veux pouvoir désactiver des produits financiers,
	afin de ne plus les voir car je ne veux pas les gérer.
	Critères d'acceptation:
		- Je dois posséder au moins un produit financier
		- La désactivation (ainsi que le fait qu'il disparaisse) doit se faire immédiatement sans déconnexion
		- les produits désactivés doivent rester désactivés même après une deconnexion puis reconnexion 
  
	#### Réactivations de produits financiers:
  	- En tant que client possédant des produits financiers dans son portefeuille,
	je veux pouvoir réactiver le		produits qui sont désactivés,
	afin de pouvoir les voir et le gérer.
	Critères d'acceptation:
		- Je dois avoir au moins un produit non-activé
		- La réactivation de ces produits vont se faire immédiatement
		- Les produits réactivés doivent le rester même si je me déconnecte
 
	#### Souscription à de nouveaux produits financiers:
	- En tant que titulaire d'un portefeuille financier,
	je veux pouvoir souscrire à de nouveaux produits financiers.
	Critères d'acceptation:
    	- L'application doit m'informer que j'ai souscris à un nouveau produit quand j'ouvre mon portefeuille
    	- Les produits auquels je souscris doivent être immédiatement disponible
		- Si un des produits pour lequel j'ai souscris est supprimer par l'institution financière, je dois être notifier quand j'ouvre mon portefeuille

  	### Fonctionnalité de virements
	#### Demande d'activation de la fonctionnalité:
	- En tant que titulaire d'un portefeuille,
	je veux pouvoir faire une demande,
	afin d'obtenir la fonctionnalité de virement.
	Critères d'acceptation:
		- Une fois la demande accepté, l'application doit retenir que ma demande a été accepter et ne dois pas m'enlever la fonctionnalité même lors de la déconnexion

	#### Effectuer un virement:
	- En tant que titulaire d'un portefeuille,
	je veux pouvoir effectuer un virement vers un autre compte,
	afin de transférer de l'argent sans avoir besoin d'une carte bancaire.
	Critères d'acceptation:
		- Une demande pour obtenir la fonctionnalité a déjà été introduite et acceptée par la banque
		- Le compte et le nom du destinataire doivent être spécifiés
		- Le compte depuis lequel on veut virer cet argent doit être sélectionné
		- Un montant à virer doit être précisé
		- Le nom du destinataire doit correspondre au nom du titulaire du compte de destination 
		- Le montant à virer doit être inférieur ou égal au montant sur le compte, mais aussi positif 


- Gérer première connexion
  - EN TANT QU'institution financière, JE VEUX pouvoir regarder les identifiants dans une demande de portefeuille financier d'un nouveau client AFIN de vérifier s'il est client de l'instutuion 
  - EN TANT QUE nouveau client tiulaire d'un produit financier, JE VEUX pouvoir introduire une demande d'ouverture de portefeuille financier à une institution financière les détenant AFIN de gérer les opérations concernant mes produits
- Accéder au portefeuille
  - EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir visualiser mon portefeuille AFIN de gérer mes produits  
    #### Critères d'acceptation : 
    -   Le client doit être connecté à l'application 
    - Le client détient au moins un produit financier dans une institution financière
-  Visualiser historique
    -  EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir visualiser l'historique de mes produits
     AFIN de faire des opérations sur celles-ci 
        #### Critères d'acceptation : 
        -   Le client doit avoir au moins un portefeuille 
        - Le client doit être connecté
-  Filtrer historique
    - EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir filtrer l'historique selon une certaine période, certains produits financiers ou encore un ensemble de portefeuilles
AFIN de comparer les données dans le temps ou trouver certaines transactions
        #### Critères d'acceptation : 
      -   Le client détient au moins un portefeuille
      - Le client doit être connecté
- Exporter données
    -  EN TANT QUE client, JE VEUX pouvoir exporter l'historique au format CSV AFIN de pouvoir l'imprimer ou le partager 
        #### Critères d'acceptation : 
       - Toute donnée filtrée est comprise dans l'historique uniquement
       - Le client détient au moins un portefeuille
       - Le client doit être connecté
- Changer de type de visualisation
    - EN TANT QUE client, JE VEUX pouvoir changer le format de la visualisation de mes produits (graphes, listes, tableaux,...)
        #### Critères d'acceptation : 
      - Le client détient au moins un portefeuille
      - Le client doit être connecté
- Visualiser portefeuille
  - EN TANT QUE client, JE VEUX pouvoir visualiser les produits financiers de mon portefeuille AFIN de voir l'évolution des cours de ceux-ci   
    #### Critères d'acceptation : 
    -   Le client détient au moins un portefeuille
    - Le client doit être connecté
- Sélectionner produits à visualiser
  - EN TANT QUE client, JE VEUX pouvoir sélectionner mes produits à visualiser AFIN de comparer certains produits uniquement
    #### Critères d'acceptation :
    - Les produits sélectionnés sont des produits appartenant au client
    - Le client doit être connecté
- Changer de portefeuille 
  - EN TANT QUE client connecté titulaire de produits financiers dans diverses institutions, JE VEUX pouvoir changer de portefeuille AFIN de voir mes différents produits dans diverses institutions  
       #### Critères d'acceptation : 
    -   Le client détient au moins 2 portefeuilles 
    - Le client doit être connecté
## Session
- Se connecter
  - EN TANT QUE client, JE VEUX pouvoir me connecter à l'application client AFIN d'avoir accès à mes données
    #### Critères d'acceptation : 
     - Le client ne peut pas se connecter à 2 appareils différents simultanément
- Exécution session
  - EN TANT QUE client, JE VEUX pouvoir exécuter la session AFIN de faire différentes actions sur l'application client 
     #### Critères d'acceptation :
    - Le client doit être connecté 
-   Réinitialiser mot de passe
    - EN TANT QUE client, JE VEUX pouvoir réinitialiser mon mot de passe AFIN de me protéger d'un futur oubli ou d'une fuite de données
        #### Critères d'acceptation : 
      - Le client doit être connecté
      - Le client doit connaître son mot de passe pour le changer

# Application bancaire
## Session
- Traiter une demande 
  - EN TANT QU'institution financière, JE VEUX pouvoir regarder les identifiants dans une demande de portefeuille financier d'un nouveau client AFIN de vérifier s'il est client de l'institution et poursuivre la procédure de réponse à cette demande
    #### Critères d'acceptation : 
     - 1
      - 2

## Clients

## Virements

## Produits financiers




