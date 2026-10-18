# TechStock — fiabiliser un catalogue informatique

Fiabiliser le chiffre d’affaires, identifier les références prioritaires et distinguer anomalies de données, prix atypiques légitimes et risques de stock.

## Mon approche

Je contrôle la qualité des données et les clés avant de calculer les indicateurs. Je compare les résultats, explicite les hypothèses et propose des actions à vérifier avec le métier. Ce projet utilise des données synthétiques et ne correspond à aucune mission réelle.

## Méthodes

- Audit de rapprochement ERP/web, exclusions tracées et réconciliation des montants au périmètre valide.
- Distributions, quantiles, MAD sur log-prix par catégorie et contrôle IQR.
- Analyse ABC/Pareto, contribution à la marge, saisonnalité descriptive et croisements avec le stock.
- Matrice d’action contribution×couverture, seuils explicites et priorisation de vérification.

## Livrables

- [Notebook Jupyter](notebooks/analyse.ipynb) : calculs exécutés, graphiques et analyse détaillée.
- [Rapport PowerPoint](presentation/soutenance.pptx) : présentation modifiable.
- [Rapport PDF](presentation/soutenance.pdf) : version de lecture.
- [Synthèse des résultats](analysis/SYNTHESE.md).
- `data/` et `analysis/` : sources, tables nettoyées et résultats au format CSV.

## Reproduire l’analyse

Installer Python 3.12 et les dépendances avec `python -m pip install -r requirements.txt`. Ouvrir le notebook dans Jupyter ou VS Code, choisir le noyau Python installé et exécuter toutes les cellules dans l’ordre. La graine de simulation est fixe. Les sources sont régénérées à l’exécution ; ne pas remplacer ces CSV par des données réelles sans adapter le chargement.

La dernière cellule recrée le PowerPoint. Pour actualiser le PDF après modification, ouvrir la présentation dans PowerPoint ou LibreOffice Impress puis l’exporter en PDF. Les graphiques sont des images et les textes restent modifiables.

Les données fictives, les méthodes et les limites sont détaillées dans le notebook. Les résultats ne constituent pas une performance démontrée en situation réelle.

## Aperçu

![Graphique de l’analyse](reports/ca_et_marge_mensuels.png)

## Quelques repères

Ces valeurs décrivent le jeu synthétique utilisé dans ce projet.

| Indicateur | Valeur |
|---|---:|
| lignes valides | 117 080 |
| liaisons ambigues | 40 |
| ca net | 83 890 298,0600 |
| marge commerciale | 61 175 149,9400 |
