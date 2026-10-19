# Séance 4 : Tâches évaluées

Thème : Google Sheets (1) : tableaux, formules de base, mise en forme

<nav class="page-nav">
  <a href="cours_seance_04.html">← Cours</a>
  <a href="../../index.html">Accueil</a>
</nav>

## Tâche : Remplir le Sheet partagé (2 points)

Ouvrez le Google Sheets du dossier partagé en séance 2 (celui où l'enseignant était lecteur). Travaillez dans ce fichier, pas de second Sheet.

1. Nom du fichier : doit contenir une date au format `YYYY-MM-DD_…` (clic sur le titre en haut à gauche) ; ex. `2026-10-26_OutilsInfo_mesures-sheets`
2. Droits enseignant sur ce même fichier : invitez `shuraux@he2b.be` en Éditeur (droits d'édition complets sur le fichier). Vous restez propriétaire : ne transférez pas la propriété. Si l'enseignant est encore seulement lecteur, remontez le rôle fichier par fichier (ne vous fiez pas seulement à l'héritage du dossier).
3. Feuille renommée `Mesures` : tableau avec en-têtes en ligne 1 : Date, Poste, Grandeur, Valeur, Unité, Valeur corrigée. Au moins 12 lignes de données (mesures de labo fictives). Une ligne = un enregistrement ; pas de fusion dans la zone de données.
4. Mise en forme : format nombre cohérent sur Valeur et Valeur corrigée ; bordures utiles ; Affichage → Figer → 1 ligne.
5. Une cellule fixe (ex. sur une feuille `Params` ou hors tableau) contient un facteur numérique. La colonne Valeur corrigée calcule `Valeur × facteur` avec une référence absolue `$`, puis recopiez la formule vers le bas avec la poignée.
6. Deuxième feuille `Synthese` dans le même fichier : libellés + formules SOMME, MOYENNE, MIN, MAX, et NB ou NBVAL qui pointent vers la feuille `Mesures` (ex. `=SOMME(Mesures!D2:D13)`), pas de résultats tapés à la main.

L'enseignant vérifie dans Drive (droits éditeur sur ce Sheet, contenu des feuilles).

**Deadline : la veille de la prochaine séance, 20:00**

<nav class="page-nav">
  <a href="cours_seance_04.html">← Cours</a>
  <a href="../../index.html">Accueil</a>
</nav>

<footer class="site-footer"><a href="mailto:shuraux@he2b.be">Sylvain Huraux - HE2B - ISIB</a></footer>
