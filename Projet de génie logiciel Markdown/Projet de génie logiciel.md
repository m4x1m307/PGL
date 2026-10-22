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
		
- Portefeuille 
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

	Fonctionnalité de modification du portefeuille:
		Désactivation de produits financiers:
			En tant que titulaire d'un portefeuille financier possédant des produits,
			je veux pouvoir désactiver des produits financiers,
			afin de ne plus les voir car je ne veux pas les gérer.
			Critères d'acceptation:
			- Je dois posséder au moins un produit financier
			- La désactivation (ainsi que le fait qu'il disparaisse) doit se faire immédiatement sans déconnexion
			- les produits désactivés doivent rester désactivés même après une deconnexion puis reconnexion 
  
		Réactivations de produits financiers:
  			En tant que client possédant des produits financiers dans son portefeuille,
			je veux pouvoir réactiver les produits qui sont désactivés,
			afin de pouvoir les voir et les gérer.
			Critères d'acceptation:
			- Je dois avoir au moins un produit non-activé
			- La réactivation de ces produits vont se faire immédiatement
			- Les produits réactivés doivent le rester même si je me déconnecte
 
		Souscription à de nouveaux produits financiers:
			En tant que titulaire d'un portefeuille financier,
			je veux pouvoir souscrire à de nouveaux produits financiers.
			Critères d'acceptation:
			- L'application doit m'informer que j'ai souscris à un nouveau produit quand j'ouvre mon portefeuille
			- Les produits auquels je souscris doivent être immédiatement disponible
			- Si un des produits pour lequel j'ai souscris est supprimer par l'institution financière, je dois être notifier quand j'ouvre mon portefeuille

  	Fonctionnalité de virements:
		Demande d'activation de la fonctionnalité:
			En tant que titulaire d'un portefeuille,
			je veux pouvoir faire une demande,
			afin d'obtenir la fonctionnalité de virement.
			Critères d'acceptation:
			- Une fois la demande accepté, l'application doit retenir que ma demande a été accepter et ne dois pas m'enlever la fonctionnalité même lors de la déconnexion

		Effectuer un virement:
			En tant que titulaire d'un portefeuille,
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
  
  -  EN TANT que client connecté titulaire de produits financiers, JE VEUX pouvoir sélectionner certains produits financiers à visualiser AFIN de me focaliser sur une partie de mes produits 
-  Visualiser historique
    - EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir visualiser l'historique de mes produits financiers
    -  EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir visualiser l'historique de mes produits
     AFIN de faire des opérations sur celles-ci 
    -  EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir exporter l'historique au format CSV
 AFIN de pouvoir l'imprimer ou le partager 
    - EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir filtrer l'historique selon une certaine période, certains produits financiers ou encore un ensemble de portefeuilles
AFIN de comparer les données dans le temps ou trouver certaines transactions
    - EN TANT QUE client connecté titulaire de produits financiers, JE VEUX pouvoir changer le format de la visualisation de mes produits (graphes, listes, tableaux,...)
  - Changer de portefeuille 
    - EN TANT QUE client connecté titulaire de produits financiers dans diverses institutions, JE VEUX pouvoir changer de portefeuille AFIN de voir mes différents produits dans diverses institutions
    
  -  Réinitialiser mot de passe
        - EN TANT QUE client connecté, JE VEUX pouvoir réinitialiser mon mot de passe AFIN de me protéger d'un futur oubli ou d'une fuite de données
        