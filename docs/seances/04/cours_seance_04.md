---
marp: true
theme: outils-info-ia
title: "Séance 4 — Google Sheets"
paginate: true
header: "Outils Info & IA — Séance 4 [Sylvain Huraux - HE2B - ISIB](mailto:shuraux@he2b.be)"
footer: "[← Retour à l'accueil](../../index.html)"
---

## Séance 4

Google Sheets

[→ Quiz](quiz_seance_04.html)
[→ Exercices](exercices_seance_04.html)

---

## Objectifs de la séance

- Organiser des données en **tableau propre** (une ligne = un enregistrement)
- Utiliser formules de base : `SUM`, `AVERAGE`, `IF`, `VLOOKUP` / `XLOOKUP`
- Références relatives vs absolues (`A1` vs `$A$1`)
- Mettre en forme (nombres, filtres, validation)
- Créer un graphique lisible

---

## Quand utiliser Sheets ?

| Besoin | Outil |
| --- | --- |
| Calculs, listes, suivis, notes | **Sheets** |
| Texte long, rapport | Docs |
| Présentation orale | Slides |

Sheets = tableur collaboratif. Pensez **données structurées**, pas « page Word en cellules ».

---

## Hygiène des données

Règles d'or :

1. **Une feuille** « données brutes », une autre « calculs / dashboard »
2. Ligne 1 = en-têtes
3. Pas de cellules fusionnées dans la zone de données
4. Un type par colonne (nombres / dates / texte)
5. Pas d'espaces parasites dans les nombres

---

## Références

| Écriture | Comportement à la copie |
| --- | --- |
| `B2` | relative — se décale |
| `$B$2` | absolue — fixe |
| `$B2` / `B$2` | mixte |

Exemple moyenne pondérée : poids en `$B$1`, notes en colonne relative.

---

## Formules essentielles

```text
=SUM(B2:B20)
=AVERAGE(C2:C20)
=IF(D2>=10;"Réussi";"Échoué")
=COUNTIF(E2:E50;"absent")
```

Commencez toujours par `=`. Vérifiez les plages (évitez toute la colonne si inutile).

---

## Recherche dans une table

Cas typique : retrouver le nom d'un étudiant à partir d'un matricule.

- `VLOOKUP` / `XLOOKUP` (selon disponibilité)
- Table de référence à gauche / clé unique
- Gérer le cas « introuvable » (`IFERROR`)

Ne dupliquez pas manuellement ce qu'une formule peut retrouver.

---

## Filtres et tris

1. Sélectionner le tableau
2. Données → **Créer un filtre**
3. Filtrer par cours, statut, date…

Pour un suivi de projet : filtres + couleurs conditionnelles sur « En retard ».

---

## Validation des données

Évitez les saisies libres anarchiques :

- Liste déroulante : `À faire / En cours / Fait`
- Plage numérique : note entre 0 et 20
- Date valide uniquement

Résultat : statistiques fiables.

---

## Graphiques utiles

Checklist :

- Un message clair (titre du graphique)
- Axes étiquetés + unités
- Pas de 3D ni d'effets inutiles
- Couleurs contrastées
- Source des données visible (feuille / plage)

Préférez barres / lignes ; réservez le camembert aux parts d'un tout.

---

## Collaboration sur Sheets

- Verrouiller des plages (protéger la feuille de formules)
- Commenter une cellule pour une anomalie
- Une convention : **qui saisit quoi** (éviter deux éditeurs sur la même cellule)

Historique de versions = filet de sécurité.

---

## Exemple fil rouge : suivi de notes

Colonnes : `Matricule | Nom | Labo1 | Labo2 | Labo3 | Moyenne | Statut`

- `Moyenne` = formule
- `Statut` = `IF` sur le seuil
- Graphique : distribution des moyennes
- Filtre : afficher seulement « Échoué »

---

## Pour la prochaine séance

- Construire un petit Sheet de suivi (formules + 1 graphique)
- **Séance 5 :** Google Slides (structure d'une présentation claire)
