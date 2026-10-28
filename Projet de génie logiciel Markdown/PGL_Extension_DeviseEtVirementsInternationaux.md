# Étudiant affecté à cette extension : Maxime Lawson 
# Application cliente
## Portefeuille
- Sélectionner compte bancaire
    - En tant que client,
    je veux pouvoir sélectionner un compte bancaire,
    afin d'y consulter mon solde.
        #### Critères d'acceptation :
        - Le client a déjà créé au moins un compte bancaire
- Modifier devises du compte
    - En tant que client,
    je veux pouvoir modifier les devises de mon compte bancaire,
    afin de ne plus avoir la devise par défaut ou d'avoir un compte multidevises.
        #### Critères d'acceptation :
        - Le client a déjà créé un compte bancaire
        - L'application permet de sélectionner parmi les devises disponibles
- Créer un nouveau compte bancaire
    - En tant que client,
    je veux pouvoir créer un compte bancaire,
    afin d'y stocker de l'argent ou de faire des virements.
        #### Critères d'acceptation :
        - Le client a déjà fait une demande pour créer le compte à la banque au préalable, et elle a été acceptée
        - Le client a au moins un portefeuille
- Sélectionner devises du compte
    - En tant que client possesseur d'un compte dans une institution financière,
    je veux pouvoir changer la devise principale de mon compte ou rajouter des devises dans celui ci,
    afin d'avoir un compte multidevises ou d'avoir un compte avec une devise différente de l'euro pour pouvoir faire des virements internationaux.
        #### Critères d'acceptation :
        - Le client doit avoir le choix parmi au moins 5 devises dont l'euro (EUR), le dollar américain (USD) et le livre sterling(GBP)
        - Le choix de la ou des devise(s) du compte du client doit/doivent être retenue(s) et il ne dois pas le respécifier quand il se reconnecte
## Taux des devises
- Calculer taux de conversion entre devises 
    - En tant qu'utilisateur,
    je veux calculer les taux de conversion entre des devises,
    afin de voir si une transaction entre ces devises peut être intéressante.
        #### Critères d'acceptation :
        - L'application doit montrer les différentes devises pour lesquelles le client peut calculer le taux de conversion
- Calculer taux de conversion entre devises 
    - En tant qu'API,
    je veux calculer les taux de conversion entre des devises,
    afin que l'utilisateur puisse obtenir ces taux et en faire ce qu'il veut.
        #### Critères d'acceptation :
        - Les devises pour le calcul doivent être spécifiées 
- Suivre historique des taux des devises
    - En tant qu'utilisateur,
    je veux pouvoir suivre l'historique des taux des devises,
    afin de savoir quand est ce que les devises de mon choix sont les plus intérressantes
        #### Critères d'acceptation :
        - L'application doit permettre au client de choisir les devises qu'il veux visualiser via un sélecteur
        - La visualitation doit changer en même temps que il change la devise dans le champ
## Virements
- Effectuer virement impliquant des devises
    - En tant qu'utilisateur,
    je veux pouvoir effectuer des virements impliquant des devises différentes,
    afin d'envoyer de l'argent vers un compte dans une autre devise.
        #### Critères d'acceptation :
        - Le compte source et le compte destination utilisent des devises différentes
- Appliquer taux de conversion
    - En tant qu'utilisateur effectuant un virement avec plusieurs devise,
    je veux avoir le taux de conversion qui est appliqué,
    afin de savoir combien est ce que je vais réellement payer lors de la transaction.
        #### Critères d'acceptation
        - Une fois le taux de conversion appliqué, le client ne veux pas que la conversion change pendant qu'il suis en train de faire une procédure de virement
- Appliquer frais de conversion
    - En tant qu'utilisateur effectuant un virement avec plusieurs devise,
    je veux avoir les frais de conversion appliqués,
    afin de savoir le montant de frais que je vais devoir payer.
        #### Critères d'acceptation :
        - Les frais de conversions seront réduit si c'est un virement entre différents compartiments d’un compte multidevises.
        - Le client doit bien être informé de ces frais de conversions avant d'effectuer le virement
- Préciser adresse du destinataire et numéro SWIFT de sa banque
    - En tant qu'utilisateur,
    je veux pouvoir préciser l'adresse du destinaitaire ainsi que le numéro SWIFT de sa banque,
    afin d'effectuer un virement vers ce destinaire dont le compte se trouve hors de la zone SEPA.
        #### Critères d'acceptation :
        - La banque du destinataire doit être situé hors zone SEPA
- Préciser répartition des frais de commissions
    - En tant qu'utilisateur faisant un virement impliquant des devises différentes,
    je veux pouvoir choisir comment est ce que les frais de commissions seront répartis entre le destinataire et moi,
    afin d'être en accord avec le destinataire et que le virement se déroule au mieux.
        ####  Critères d'acceptation :
        - L'application propose de sélectionner entre trois options possibles : Payer tous les frais, les destinataire payes tous les frais, ou les frais sont partagés entre les deux parties

# Application bancaire
## Visualitation
- Visualiser historique
  - En tant qu'institution financière,
  je veux pouvoir visualiser l'historique de certaines données,
  afin de faire des opérations sur celles-ci.
    #### Critères d'acceptation : 
    - L'application propose quelle données visualiser
- Exporter données
    -  En tant qu'institution financière,
    je veux pouvoir exporter l'historique au format CSV ou JSON,
    afin de pouvoir l'imprimer ou le partager.
        #### Critères d'acceptation : 
       - Toute donnée filtrée est comprise dans l'historique uniquement
- Visualiser historique des frais de commissions
    - En tant qu'institution financière,
    je veux pouvoir visualiser l'historique des frais de commissions,
    afin de voir comment les frais de commissions ont variés.
        #### Critères d'acceptation :
        - Seul les frais de commissions par défaut seront affichés si aucune modifications n'as été faite
- Visualiser historique des taux de conversions
    - En tant qu'institution financière,
    je veux pouvoir visualiser l'historique des taux de de conversion entre des devises,
    afin de voir comment est ce que le taux de conversion a varié.
        #### Critères d'acceptation :
        - Lorsque l'institution visualise l'historique, le taux de conversion ne doit pas changer
- Sélectionner période de visualisation
    - En tant qu'institution financière,
    je veux pouvoir sélectionner la période de visualisation de l'historique,
    afin de visualiser l'historique durant la période que je désire.
        #### Critères d'acceptation :
        - L'application propose certaines périodes prédéfinie (mensuel, annuel, etc...)
        - L'institution ne peux pas sélectionner une période plus récente que la date du jour
- Sélectionner devise de référence et autres devises
    - En tant qu'institution financière,
    je veux pouvoir sélectionner une devise de référence et d'autres devise pour la visualisation,
    afin de voir au mieux la variation du taux de conversion pour les devises que je désire.
        #### Critères d'acceptation :
        - L'application propose de d'abord choisir la devise de référence, et on peut ensuite sélectionner plusieurs autre devise
- Changer format d'exportation 
    - En tant qu'institution financière,
    je veux pouvoir changer le format d'exportation en JSON ou CSV,
    afin qu'il convienne le mieux à mes besoins.
        #### Critères d'acceptation :
        - L'application propose un petit menu de sélection pour choisir son format
## Pourcentage de frais de commission
- Gérer pourcentage de frais de commission
    - En tant qu'institution financière,
    je veux gérer le pourcentage de frais de commission,
        #### Critères d'acceptation :
        - C'est possible uniquement si c'est une transaction qui demande une conversion entre devises
- Modifier pourcentage de frais de commission
    - En tant qu'institution financière,
    je veux pouvoir modifier le pourcentage de frais de commission,
    afin qu'il s'adapte au mieux à la satistfaction client et la concurence
        #### Critères d'acceptation :
        - Le nouveau pourcentage s'applique uniquement aux transactions demandant une conversion entre devises
        - Par défaut, la modification s'applique à toutes les paires de devises
- Préciser pourcentage de frais de commission
    - En tant qu'institution financière,
    je veux préciser le pourcentage de frais de commission,
    afin que mes clients sachent exactement quels sont les frais de commissions appliqués pour le moment.
        #### Critères d'acceptation :
        - Préciser si les frais sont différents en fonction des paires de devises ou du type de carte utilisé pour la transaction
- Préciser la/les paire(s) de devises touchée(s) par la modification
    - En tant qu'institution financière,
    je veux préciser certaines paires de devises touchées par la modification du pourcentage de frais de commission,
    afin de volontairement cibler des paires de devises et obtenir plus de transactions les concernant.
        #### Critères d'acceptation :
        - L'application permet une option pour ne pas appliquer la modification de pourcentage sur toutes les paires de devises et selectionner celles qu'on veut
