# Extension : Gestion du budget financier

# Application cliente

## Virements récurrents

### Ajouter un virement récurrent

En tant que titulaire du portefeuille, je veux ajouter un virement automatique récurrent afin d'automatiser mes transferts d'argent.

Critères d'acceptation :
- Le titulaire peut définir les comptes source et destination, le montant et la récurrence du virement.
- L'application permet notamment de transférer automatiquement une somme fixe du compte courant vers le compte épargne à la fin du mois.
- Un virement actif s'exécute automatiquement lorsque son déclencheur et ses éventuelles conditions sont satisfaits.

### Définir une condition d'exécution

En tant que titulaire du portefeuille, je veux définir une condition d'exécution afin qu'un virement automatique soit effectué uniquement lorsque cette condition est satisfaite.

Critères d'acceptation :
- Le titulaire peut conditionner un transfert vers son épargne à la présence d'un solde suffisant sur son compte courant.
- Le titulaire peut configurer un transfert vers son compte courant lorsque celui-ci risque de devenir négatif.
- Le virement conditionnel ne s'exécute pas lorsque sa condition n'est pas satisfaite.

### Supprimer un virement récurrent

En tant que titulaire du portefeuille, je veux supprimer un virement récurrent afin d'arrêter définitivement ses prochaines exécutions.

Critères d'acceptation :
- Le titulaire peut sélectionner un virement récurrent existant et le supprimer.
- Après sa suppression, ce virement ne s'exécute plus automatiquement.

### Mettre en pause un virement récurrent

En tant que titulaire du portefeuille, je veux mettre un virement récurrent en pause afin de suspendre temporairement les transferts sans supprimer sa configuration.

Critères d'acceptation :
- Le titulaire peut mettre en pause un virement récurrent actif.
- Aucune exécution automatique de ce virement n'a lieu pendant la pause.
- La configuration du virement est conservée pour permettre sa réactivation.

### Réactiver un virement récurrent

En tant que titulaire du portefeuille, je veux réactiver un virement récurrent en pause afin de reprendre les transferts automatiques.

Critères d'acceptation :
- Le titulaire peut réactiver un virement précédemment mis en pause.
- Le virement reprend ses exécutions selon sa configuration et ses éventuelles conditions.

### Associer une catégorie à un virement récurrent

En tant que titulaire du portefeuille, je veux associer une catégorie à un virement récurrent afin que les transactions produites soient automatiquement classées.

Critères d'acceptation :
- Le titulaire peut sélectionner une catégorie existante et l'associer au virement récurrent.
- Chaque nouvelle transaction issue de ce virement est automatiquement classée dans la catégorie associée.

## Catégories et classification des transactions

### Créer une catégorie

En tant que titulaire du portefeuille, je veux créer une catégorie afin d'organiser mes transactions selon mes besoins.

Critères d'acceptation :
- Des catégories prédéfinies sont disponibles, notamment santé, travail, loisirs, sport, énergie, transport, études et autres.
- Le titulaire peut définir de nouvelles catégories.
- Chaque catégorie possède un code couleur et une icône associés.
- Une catégorie créée peut être utilisée pour classifier des transactions.

### Modifier une catégorie

En tant que titulaire du portefeuille, je veux modifier une catégorie afin d'adapter la classification à mes besoins.

Critères d'acceptation :
- Le titulaire peut sélectionner et modifier une catégorie existante.
- La catégorie modifiée conserve un code couleur et une icône associés.
- Les modifications sont prises en compte dans les affichages utilisant cette catégorie.

### Catégoriser une transaction

En tant que titulaire du portefeuille, je veux attribuer une catégorie à une transaction afin d'identifier la nature de mes dépenses et de mes revenus.

Critères d'acceptation :
- Le titulaire peut classifier aussi bien un montant payé qu'un montant reçu.
- Il peut choisir une catégorie prédéfinie ou une catégorie qu'il a créée.
- La catégorie attribuée est prise en compte dans l'historique et les analyses du budget.

### Définir des règles de classification automatique

En tant que titulaire du portefeuille, je veux définir des règles de classification automatique afin d'éviter de catégoriser manuellement chaque transaction.

Critères d'acceptation :
- Le titulaire peut associer une ou plusieurs règles à un portefeuille et à une catégorie.
- Une règle permet de comparer un attribut d'une transaction à une valeur définie.
- Les critères peuvent notamment porter sur le compte de l'émetteur ou du bénéficiaire, le montant ou le message de la transaction.
- Les transactions correspondant aux règles sont automatiquement classées dans la catégorie associée.

### Consulter l'historique par catégorie

En tant que titulaire du portefeuille, je veux consulter mon historique en tenant compte des catégories afin de comprendre la répartition de mes transactions.

Critères d'acceptation :
- L'historique et ses visualisations prennent en compte les catégories attribuées aux transactions.
- Les catégories peuvent être distinguées grâce à leur couleur et leur icône.
- Les transactions classées manuellement ou automatiquement sont prises en compte.

## Analyse du budget

### Consulter les statistiques du budget

En tant que titulaire du portefeuille, je veux consulter les statistiques de mes transactions afin de mieux comprendre mon budget.

Critères d'acceptation :
- L'application calcule le minimum et le maximum des séries de données analysées.
- Elle calcule la moyenne et l'écart type.
- Elle calcule la médiane, les quartiles et l'écart interquartile.
- Par défaut, toutes les transactions sont prises en compte.
- Les calculs respectent les catégories incluses ou exclues par le titulaire.

### Consulter les tendances du budget

En tant que titulaire du portefeuille, je veux consulter les tendances temporelles de mon budget afin de comprendre l'évolution de mes dépenses.

Critères d'acceptation :
- L'application permet de visualiser les variations saisonnières des dépenses par catégorie.
- Elle permet d'observer les tendances de croissance des dépenses.
- Elle permet notamment de comparer les dépenses de l'année précédente avec celles de l'année en cours.

### Visualiser l'état futur du portefeuille

En tant que titulaire du portefeuille, je veux visualiser une prévision de mon portefeuille à une date future afin d'anticiper ma situation financière.

Critères d'acceptation :
- Le titulaire peut choisir une date future pour la prévision.
- L'application affiche une estimation de l'état du portefeuille à cette date.
- La prévision tient compte des statistiques disponibles et des virements automatiques configurés.
- Le titulaire peut sélectionner les catégories à inclure ou à exclure de la prévision.
- La prévision est actualisée lorsque cette sélection change.

### Sélectionner les catégories à inclure ou exclure

En tant que titulaire du portefeuille, je veux sélectionner les catégories prises en compte afin d'adapter les statistiques et les prévisions à mon analyse.

Critères d'acceptation :
- Le titulaire peut inclure ou exclure des catégories pour le calcul des statistiques.
- Le titulaire peut inclure ou exclure des catégories pour la prévision de l'état futur du portefeuille.
- Les résultats sont actualisés en fonction de la sélection.
- Pour les statistiques, toutes les transactions sont considérées par défaut.

### Recevoir une alerte de dépense inhabituelle

En tant que titulaire du portefeuille, je veux recevoir une alerte lorsqu'une dépense inhabituelle est détectée afin de repérer une évolution préoccupante de mon budget.

Critères d'acceptation :
- L'application détecte des dépenses anormalement élevées par rapport à l'historique du budget.
- Elle permet également de détecter des anomalies de dépenses énergétiques par rapport à un foyer moyen.
- Une anomalie détectée peut déclencher une notification au titulaire.
- L'application peut notamment notifier une augmentation inhabituelle des dépenses d'électricité.
