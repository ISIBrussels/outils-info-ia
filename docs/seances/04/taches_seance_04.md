# Séance 4 — Tâches évaluées

**Thème :** Google Sheets  
**Objectif :** construire un tableau de suivi utilisable (pas une grille décorative)  

<nav class="page-nav">
  <a href="cours_seance_04.html">← Cours</a>
  <a href="../../index.html">Accueil</a>
</nav>

## Travail 1 — Suivi de notes / labos (obligatoire)

Créez un Google Sheet nommé :

`AAAA-MM-JJ_OutilsInformatiques_Nom_suivi_notes`

Feuille `Donnees` avec colonnes :

| Matricule | Nom | Labo1 | Labo2 | Labo3 | Moyenne | Statut |
| --- | --- | --- | --- | --- | --- | --- |

Consignes :

1. Au moins **8 lignes** de données fictives mais réalistes (notes /20)
2. `Moyenne` = formule (`AVERAGE` ou moyenne pondérée si vous allez plus loin)
3. `Statut` = formule `IF` : `Réussi` si moyenne ≥ 10, sinon `Échoué`
4. Ligne 1 = en-têtes ; **pas** de fusion dans la zone de données
5. Activez un **filtre** sur le tableau

## Travail 2 — Validation et mise en forme

1. Ajoutez une colonne `Remarque` avec **liste déroulante** : `OK` / `À revoir` / `Absent`
2. Format nombre à 1 décimale pour les moyennes
3. Mise en évidence conditionnelle : lignes `Échoué` visibles d’un coup d’œil

## Travail 3 — Graphique

1. Créez un graphique (barres ou histogramme) des moyennes
2. Titre clair : `Distribution des moyennes — groupe [X]`
3. Axes lisibles ; pas de 3D
4. Placez le graphique dans une feuille `Dashboard` (option recommandée)

## Travail 4 — Partage

Partagez le Sheet avec votre binôme en **éditeur** et ajoutez un commentaire sur une cellule suspecte (ex. note hors plage).

## Critères de réussite

| Critère | Attendu |
| --- | --- |
| Formules | Moyenne + Statut automatiques |
| Qualité données | En-têtes, filtre, validation |
| Graphique | Titré et lisible |
| Collab | Partage + au moins 1 commentaire |

<nav class="page-nav">
  <a href="cours_seance_04.html">← Cours</a>
  <a href="../../index.html">Accueil</a>
</nav>

<footer class="site-footer"><a href="mailto:shuraux@he2b.be">Sylvain Huraux - HE2B - ISIB</a></footer>
