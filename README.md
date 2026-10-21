# Étude solaire — Bâtiment SOECO, Dakar

Calculateur interactif de dimensionnement photovoltaïque pour un bâtiment tertiaire
à Dakar (Sénégal), avec financement en échéances égales sans intérêt (coût + marge).

**Page :** https://reigen-kageno.github.io/soeco-solar-study/

## Ce que fait l'outil

Six paramètres ajustables — puissance PV, batterie, consommation annuelle, durée de
financement, marge, hausse tarifaire — recalculent en direct :

- la couverture solaire mois par mois, contre la consommation réelle du bâtiment ;
- ce que le client sort chaque mois : mensualité solaire + facture SENELEC restante ;
- la saturation du système sans revente réseau, et le gain marginal de chaque kWc ajouté ;
- l'économie cumulée sur 60 mois ;
- la courbe de charge horaire et la puissance de pointe.

## Méthode

- **Productible** : PVGIS, Dakar (14,72° N, 17,47° O), inclinaison 17°, pertes 14 %.
- **Consommation** : factures SENELEC + index relevés + mesures par pinces de courant.
- **Structure tarifaire** : tranches SENELEC reconstituées et vérifiées sur factures (±0,61 %).
- **Coût marginal d'un kWh déplacé** : 255,84 FCFA TTC.

## Limites assumées

La consommation de référence est une estimation recalée : le compteur sous-compte et les
pinces ne mesurent que deux phases à la fois. Le paramètre « consommation annuelle » existe
précisément pour explorer cette incertitude. Les prix d'équipement sont des ordres de grandeur
à confirmer par devis.

---

Page autonome (un seul fichier HTML, aucune dépendance externe, aucun traceur).
