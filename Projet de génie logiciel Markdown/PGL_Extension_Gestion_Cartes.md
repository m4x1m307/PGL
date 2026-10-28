# Application cliente 
## Visualisation
- Visualiser historique des cartes
   - En tant que client, je veux pouvoir visualiser l'historique de transactions de mes cartes afin de pouvoir gérer mes dépenses ou faire du monitoring
     #### Critères d'acceptation :  
       - Le client doit être connecté
      - Le client doit posséder au moins une carte bancaire
      - Le client doit détenir au moins 1 portefeuille dans une institution financière

- Changer type de visualisation de l'historique
   - En tant que client, je veux pouvoir changer le type de visualisation des cartes afin d'avoir un support visuel correspondant à mes besoins
     #### Critères d'acceptation :
        - Le client doit être connecté
      - Le client doit posséder au moins une carte bancaire
      - Le client doit détenir au moins 1 portefeuille dans une institution financière
- Filtrer historique des cartes
  - En tant que client, je veux pouvoir filtrer l'historique des cartes par période ou autres options afin de voir qu'une partie spécifique de l'historique
    #### Critères d'acceptation : 
       - Le client doit être connecté
      - Le client doit posséder au moins une carte bancaire
      - Le client doit détenir au moins 1 portefeuille dans une institution financière
- Exporter historique des cartes
  - En tant que client, je veux pouvoir exporter l'historique de mes cartes au format CSV ou JSON afin de pouvoir l'imprimer ou le partager

    #### Critères d'acceptation : 
    - Le client doit être connecté
    - Le client doit posséder au moins une carte bancaire
    - Le client doit détenir au moins 1 portefeuille dans une institution financière
## Cartes
- Gérer cartes
  - En tant que client, je veux pouvoir gérer mes cartes bancaires afin de l'adapter à mon usage personnel 
    #### Critères d'acceptation : 
    - Le client doit être connecté
    - Le client doit posséder une carte bancaire
    - Le client doit détenir au moins 1 portefeuille dans une institution financière
   
- Demander nouvelle carte
  - En tant que client, je veux pouvoir demander une nouvelle carte bancaire afin de gérer différents budgets de différents comptes
     ### Critères d'acceptation
    -  Le client doit être connecté
    - Le client doit posséder un compte dans une institution financière
    - Le client doit avoir une justification à cette demande

-  Demande de désactivation d'une carte
    - En tant que client, je veux pouvoir demander de désactiver une carte afin de bloquer enitèrement l'accès à une carte que je n'utilise plus
        ### Critères d'acceptation 
       - Le client doit posséder une carte bancaire active  lié à compte
      - Le client doit posséder un compte dans une institution financière

-  Sélectionner justification
    - En tant que client, je veux pouvoir sélectionner la raison de ma demande d'une nouvelle carte ou de désactivation de carte afin de valider ma demande et d'en informer la motivation à mon institution financière
        ### Critères d'acceptation       
       - Le client doit être connecté
        - Le client doit posséder un compte dans une instituiotion financière
    
- Associer carte au portefeuille
  - En tant que client, je veux pouvoir associer une carte bancaire à mon portefeuille afin de gérer mes transactions
    ### Critères d'acceptation
    -   Le client doit être connecté
    - Le client doit posséder au moins un compte dans une institution financière
    - Le compte associé à la carte n'est pas lié à d'autres cartes bancaires du client

 # Paramètres de la carte

- Modifier paramètres de la carte
  - En tant que client, je veux pouvoir modifier les paramètres de mes cartes bancaires afin que ceux-ci correspondent à mon usage 
    ### Critères d'acceptation 
    - Le client doit posséder une carte bancaire
    - Le client doit être connecté

-  Bloquer temporairement carte
    - En tant que client, je veux pouvoir bloquer temporairement ma carte bancaire afin de la retrouver suite à une perte ou bien interdire les transactions de celle-ci suite à une fuite de données    
      ### Critères d'acceptation 
        - Le client doit être connecté
        - La carte que le client veut bloquer doit être active

- Gérer accès de la carte à l'étranger
  - En tant que client, je veux pouvoir gérer l'accès de ma carte lorsque que je suis en déplacement hors du pays hôte de mon institution financière afin de limiter les frais d'utilisation indésirables
    ### Critères d'acceptation
    - Le client doit être connecté 
    - Le client doit détenir une carte bancaire active  

- Activer carte à l'étranger
  - En tant que client, je veux pouvoir autoriser l'utilisation de ma carte à l'étranger afin de gérer mes dépenses en déplacement
       ### Critères d'acceptation
    - Le client doit être connecté
    Le client doit possséder uene carte bancaire active
    - La carte bancaire du client doit être compatible avec l'option de transactions à l'étranger

- Désactiver carte à l'étranger
  - En tant que client, je veux pouvoir interdire l'utilisation de ma carte à l'étranger afin d'éviter des frais cachés ou des bornes de paiement frauduleuses
    ### Critères d'acceptation  
    - Le client doit être connecté 
    - Le client doit posséder une carte bancaire active
    - La carte bancaire du client doit être compatible avec l'option de transactions à l'étranger

## Crédit 
- Gérer montant mensuel du crédit
  - En tant que client, je veux gérer le montant de mon crédit mensuel afin de ne pas être surendetté
    ### Critères d'acceptation
    - Le client doit être connecté 
    - Le client doit avoir une carte de crédit active
    - Le client ne peut pas dépasser le crédit autorisé par son institution financière

- Interdire le solde négatif
  - En tant que client, je veux pouvoir bloquer les transactions qui donnent lieu à des soldes négatifs afin de ne pas m'endetter et payer des intérêts plus élevés
      ### Critères d'acceptation
    - Le client doit être connecté 
    - Le client doit avoir une carte de crédit active

- Autoriser le solde négatif
  - En tant que client, je veux pouvoir autoriser les transactions menant à un solde négatif sur ma carte de crédit afin de faire des achats conséquents sans avoir la somme exacte
      ### Critères d'acceptation
    - Le client doit être connecté 
    - Le client doit avoir une carte de crédit active
    - Le client ne peut pas dépasser le crédit autorisé par son institution financière

- Changer seuil d'une carte de crédit
  - En tant que client, je veux pouvoir changer le seuil de mes cartes de crédit afin de limiter mes dettes et d'éviter de payer trop d'intérêts 
    ### Critères d'acceptation    
    - Le client doit être connecté 
    - Le client doit avoir une carte de crédit active
    - Le client ne peut pas dépasser le crédit autorisé par son institution financière 

- Changer définitivement le seuil
  - En tant que client, je veux pouvoir changer définitivement le seuil de mes cartes de crédits afin de limiter mes dettes
      ### Critères d'acceptation
    - Le client doit être connecté à l'application client
    - Le client doit avoir une carte de crédit active
    - Le client ne peut pas dépasser le crédit autorisé par son institution financière


# Application bancaire
## Gestion des clients
- Gérer cartes clients
  - En tant qu'employé, je veux pouvoir gérer 
-les cartes de mes clients afin de pouvoir les administrer 
      ### Critères d'acceptation
    - L'employé doit être connecté à l'application bancaire
    - Le client doit avoir au moins un produit financier dans l'institution financière
    - L'employé travaille dans une institution financière 

- Procéder à la désactivation d'une carte
    - En tant qu'employé, je veux pouvoir procéder à la désactivation 
d'une carte d'un client afin de répondre à la demande de désactivation de carte d'un client
        ### Critères d'acceptation
      - L'employé travaille dans une institution financière
      - La demande de désactivation du client concerne une carte bancaire active
      - La carte va être désassociée du compte auquel elle était liée  
 
-  Gérer montant carte de crédit client
    - En tant qu'employé, je veux pouvoir gérer le montant accordé au client d'une carte de crédit afin qu'il ne dépasse une limite et que l'institution financière puisse minimiser les pertes en cas de non remboursement
        ### Critères d'acceptation
      - L'employé travaille dans une institution financière
      - Le client détient 1 carte de crédit active lié à un compte 

- Traiter demande de nouvelle carte
  - En tant qu'employé, je veux pouvoir traiter une demande de nouvelle carte afin de donner un moyen de paiement et de retrait d'argent physique au client
      ### Critères d'acceptation 
     - L'employé travaille dans une institution financière
     - Le client a donné une justification valable pour 
avoir lune nouvelle carte
     - Après 2 demandes de nouvelles cartes, le client devra payer les frais de fabrication des prochaines cartes   
    - Le client détient au moins 1 compte dans l'institution financière 

- Procéder au renouvellement d'une carte
  - En tant qu'employé, je veux pouvoir procéder au renouvellement d'une carte qui a été perdue ou volée afin de redonner accès au client à un moyen de paiement et de retrait d'argent physique 
    ### Critères d'acceptation
    - L'employé travaille dans une institution financière
    - Le client possède au moins une carte bancaire
    - L'ancienne carte bancaire sera bloquée 

- Créer nouvelle carte
  - En tant qu'employé, je veux pouvoir créer une nouvelle carte bancaire afin de faire suite à la procédure de demande d'une nouvelle carte
       ### Critères d'acceptation
    - L'employé a l'autorisation de l'institution financière de créer la carte 
    - L'employé travaille dans une institution financière
    - Le client fait partie des clients de l'institution financière de l'employé

- Bloquer ancienne carte client 
  - En tant qu'employé, je veux pouvoir bloquer l'ancienne carte bancaire d'un client afin d'interdire les transactions à partir de cette ancienne carte
    ### Critères d'acceptation
    - L'employé travaille dans une institution financière
    - L'employé a l'autorisation de l'instution financière de bloquer la carte
    - L'ancienne carte sera bloquée et inutilisable par la suite  