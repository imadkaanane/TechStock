# Mission

Le catalogue ERP compte 2 500 références ; les commandes web représentent 120 000 lignes sur trois ans. Des SKU correspondent à plusieurs produits, certaines lignes sont dupliquées et des quantités sont invalides. Le stock disponible ne décrit pas des réceptions complètes : une rotation exacte ne peut donc pas être affirmée.

## Contraintes

- Résoudre les cardinalités avant toute jointure ; ne jamais attribuer arbitrairement un SKU ambigu.
- Arrondir les montants au niveau de la ligne selon une convention explicite.
- Ne pas supprimer un prix uniquement parce qu’il est extrême ; présenter une liste d’investigation.
- Qualifier couverture et rotation de proxies lorsque le stock moyen et les réceptions sont absents.