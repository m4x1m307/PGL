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
    - En tant que 
    - 


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
        