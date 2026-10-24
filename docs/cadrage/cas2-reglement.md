# Fiche de cadrage : Questions sur le règlement intérieur

> Remplir chaque rubrique en une à trois phrases. Les rubriques marquées (obligatoire) sont vérifiées par `pytest`.

## Besoin en une phrase (obligatoire)

Répondre aux questions des utilisateurs sur le règlement intérieur en retrouvant rapidement les passages pertinents et en signalant les cas nécessitant une interprétation humaine.

## Utilisateur final (obligatoire)

Les étudiants, les enseignants et le personnel administratif utilisent l'outil pour obtenir une première réponse sur les règles de vie et de fonctionnement de l'établissement.

## Approche retenue (obligatoire)

Cocher une seule case :

- [ ] Règles métier
- [ ] Machine learning
- [x] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire, citer au moins deux critères de la grille : (a) données étiquetées, (b) vérifiabilité, (c) coût par requête, (d) conséquence d'une erreur)

La recherche augmentée par récupération utilise le règlement officiel comme source vérifiable (b), sans nécessiter un grand jeu de questions étiquetées (a). Elle limite les réponses inventées en citant les passages retrouvés, avec un coût par requête maîtrisé (c) ; les situations disciplinaires restent soumises à une validation humaine (d).

## Données nécessaires et leur origine (obligatoire)

Il faut disposer des versions validées du règlement intérieur, des procédures associées, de leur date d'entrée en vigueur et de leurs références. Les documents sont fournis par l'administration et sont découpés en passages indexables, avec leurs titres et numéros de page conservés.

## Métrique de succès et seuil d'acceptation (obligatoire)

La métrique principale est le taux de réponses dont la source est correctement retrouvée, avec un seuil d'au moins 90 % sur un jeu de 50 questions représentatives. Une réponse doit citer le passage utilisé ou indiquer qu'aucune information fiable n'a été trouvée.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Une réponse erronée peut induire une sanction injuste ou une mauvaise compréhension des droits et obligations. Les réponses concernant une sanction, une exception ou un conflit sont vérifiées par l'administration avant d'être appliquées.

## Risques éthiques ou de confidentialité (obligatoire)

Le système doit éviter de divulguer des informations personnelles contenues dans des documents internes et respecter les droits d'accès. Il doit afficher la date de la source et ne pas présenter une interprétation automatique comme une décision officielle.

## Approche écartée et pourquoi (facultatif)
