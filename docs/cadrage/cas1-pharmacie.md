# Fiche de cadrage : Ordonnances incomplètes en pharmacie

> Remplir chaque rubrique en une à trois phrases. Les rubriques marquées (obligatoire) sont vérifiées par `pytest`.

## Besoin en une phrase (obligatoire)

Détecter rapidement les avis positifs, négatifs ou ambigus concernant le service d'une pharmacie afin de prioriser les actions d'amélioration.

## Utilisateur final (obligatoire)

Le pharmacien ou le responsable qualité consulte les résultats pour repérer les problèmes récurrents et décider quelles réponses nécessitent une vérification humaine.

## Approche retenue (obligatoire)

Cocher une seule case :

- [ ] Règles métier
- [x] Machine learning
- [ ] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire, citer au moins deux critères de la grille : (a) données étiquetées, (b) vérifiabilité, (c) coût par requête, (d) conséquence d'une erreur)

L'apprentissage supervisé est adapté si des avis historiques sont étiquetés en sentiment (a), car il permet d'évaluer la qualité sur un jeu de test. Les prédictions restent vérifiables par le pharmacien (b) et le coût par requête est faible (c), mais tout avis lié à la sécurité doit être contrôlé par un humain (d).

## Données nécessaires et leur origine (obligatoire)

Des avis clients anonymisés, leur date, leur note éventuelle et une étiquette positif, négatif ou ambigu sont nécessaires. Les données proviennent des formulaires de satisfaction et des plateformes d'avis, après suppression des noms, numéros de téléphone et informations de santé.

## Métrique de succès et seuil d'acceptation (obligatoire)

La métrique principale est le macro-F1 sur un jeu de test séparé, avec un seuil d'acceptation d'au moins 0,80 et un rappel d'au moins 0,90 pour la classe négative.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Une erreur peut masquer une plainte importante ou faire perdre la confiance d'un patient. Les avis négatifs, ambigus et ceux contenant un signal de sécurité sont relus par le pharmacien avant toute action.

## Risques éthiques ou de confidentialité (obligatoire)

Les avis peuvent contenir des informations de santé ou des données identifiantes ; elles doivent être anonymisées et conservées avec un accès limité. Le modèle ne doit pas servir à établir un diagnostic médical ni à prendre seul une décision concernant un patient.

## Approche écartée et pourquoi (facultatif)
