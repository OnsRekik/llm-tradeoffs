# Cadrage

## Question
Quel modèle et quel prompt offrent le meilleur compromis
qualité / coût / latence sur une tâche de questions-réponses
avec questions sans réponse ?

## Données
- SQuAD 2.0 : échantillon de 100 questions (1/3 sans réponse), seed=42
- Jeu métier : 20-30 questions sur un corpus hydrogène/énergie (phase suivante)

## Configurations
- 3 modèles (petit, moyen, grand) x 2 prompts (simple, structuré)

## Métriques
- Qualité : Exact Match, F1, taux de refus correct, LLM-as-judge
- Coût par requête, latence médiane

## Critères de réussite
- 6 configurations comparées, dashboard déployé avec lien public,
  README complet avec 2-3 chiffres clés

## Hors périmètre (phase 1)
- Fine-tuning, authentification, base de données lourde

## Risques
- Contamination de SQuAD par l'entraînement des modèles
- Échantillon petit : écarts de quelques points non significatifs
- Juge LLM trop indulgent
- Budget API
