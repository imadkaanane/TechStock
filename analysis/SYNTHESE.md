# TechStock — qualité, catalogue et stock

Fiabiliser ERP/web et identifier les références à surveiller.

## Résultats
- 40 liaisons ambiguës exclues avant jointure pour éviter une multiplication des ventes.
- 6 prix atypiques détectés sur log-prix par catégorie, signalés et conservés.

## Actions
- Résoudre les SKU ambigus avec le référentiel métier.
- Prioriser les références A et examiner les couvertures longues.

## Limites
- Prix extrêmes potentiellement légitimes : pas de suppression automatique.
- Stock initial comme proxy : rotation comptable impossible sans stock moyen et réceptions.
- Données fictives, marge hors frais fixes et logistique.
