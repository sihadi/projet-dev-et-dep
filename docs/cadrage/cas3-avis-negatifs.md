# Fiche de cadrage : Priorisation des avis négatifs

> Remplir chaque rubrique en une à trois phrases. Les rubriques marquées (obligatoire) sont vérifiées par `pytest`.

## Besoin en une phrase (obligatoire)

Classer et prioriser les avis négatifs afin que l'équipe de l'établissement traite d'abord les problèmes les plus urgents et les plus fréquents.

## Utilisateur final (obligatoire)

Le responsable relation client ou l'équipe qualité consulte les catégories et les scores de priorité pour organiser les réponses et les actions correctives.

## Approche retenue (obligatoire)

Cocher une seule case :

- [ ] Règles métier
- [x] Machine learning
- [ ] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire, citer au moins deux critères de la grille : (a) données étiquetées, (b) vérifiabilité, (c) coût par requête, (d) conséquence d'une erreur)

L'apprentissage supervisé convient si les avis historiques sont classés par thème et niveau d'urgence (a). Les catégories et les mots importants sont vérifiables par l'équipe qualité (b), l'inférence est peu coûteuse à grande échelle (c), et une erreur de priorité peut retarder la résolution d'un problème sérieux (d), d'où une revue humaine.

## Données nécessaires et leur origine (obligatoire)

Il faut des avis anonymisés, leur date, leur note, leur catégorie (livraison, accueil, produit ou autre) et leur niveau d'urgence validé. Les données viennent des enquêtes de satisfaction et des canaux de support, avec les informations personnelles supprimées.

## Métrique de succès et seuil d'acceptation (obligatoire)

La métrique principale est le rappel des avis urgents, avec un seuil d'au moins 0,90, complété par un macro-F1 d'au moins 0,80 sur les catégories. Le tableau de résultats doit aussi permettre de retrouver les exemples classés.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Une erreur peut retarder la prise en charge d'un incident ou faire perdre un client. Les avis classés urgents et ceux dont la confiance est faible sont relus par l'équipe qualité avant la priorisation définitive.

## Risques éthiques ou de confidentialité (obligatoire)

Les données doivent être anonymisées et utilisées uniquement pour améliorer le service. Le classement ne doit pas pénaliser un auteur selon son identité, son origine ou son style d'écriture, et les seuils doivent être contrôlés régulièrement.

## Approche écartée et pourquoi (facultatif)
