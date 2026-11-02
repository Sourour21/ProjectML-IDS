# ProjectML-IDS
Explication d’un détecteur d’intrusion (UNSW-NB15) avec SHAP 

Ce projet entraîne un détecteur d'attaques réseau sur UNSW-NB15, puis explique
ses décisions (importance interne, permutation, SHAP) pour vérifier s'il apprend
de vrais comportements d'attaque ou des artefacts du jeu de données.

## Données
Jeu : UNSW-NB15 (Moustafa et Slay, 2015), page officielle de l'UNSW Canberra.
Fichiers utilisés (version « Training and Testing Sets ») :
- `UNSW_NB15_training-set.csv` (175 341 lignes)
- `UNSW_NB15_testing-set.csv` (82 332 lignes)

Les CSV ne sont pas dans le dépôt. Placez-les dans
`Mon Drive/projet1/data/` de votre Google Drive.

## Exécution
1. Ouvrir `projet1.ipynb` dans Google Colab (bouton en haut du notebook).
2. Monter Google Drive quand demandé.
3. Menu **Exécution > Redémarrer et tout exécuter**.

Durée approximative : 30 à 60 min (calcul SHAP et réglage inclus).

## Environnement
- Graine aléatoire : `SEED = 42`
- pandas X.X | scikit-learn X.X | xgboost X.X | shap X.X
  (recopiez la sortie de la première cellule du notebook)

## Résultats principaux
| Modèle | Précision | Rappel | F1 | PR-AUC |
|---|---|---|---|---|
| Régression logistique | | | | |
| Forêt aléatoire | | | | |
| XGBoost | | | | |

Ablation (forêt, sans sttl/dttl/ct_state_ttl) : PR-AUC passe de X à Y.

## Conclusion
(2 à 3 phrases qui répondent à la question centrale.)

## Références
- Moustafa & Slay (2015), UNSW-NB15, MilCIS.
- Sarhan et al. (2020-2021) sur les variables TTL.
- Arp et al. (2022), Dos and Don'ts of ML in Computer Security.
