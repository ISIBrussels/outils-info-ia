---
marp: true
theme: outils-info-ia
title: "Séance 4 : Google Sheets (1)"
paginate: true
header: "Outils Info & IA : Séance 4 [Sylvain Huraux - HE2B - ISIB](mailto:shuraux@he2b.be)"
footer: "[← Retour à l'accueil](../../index.html)"
---

## Séance 4

Google Sheets (1)

Tableaux, formules de base, mise en forme

---

## Objectifs de la séance

- Créer un **tableau propre** (en-têtes, une ligne = un enregistrement)
- Saisir des **données** typées : texte, nombres, dates
- Mettre en forme : nombres, alignement, bordures, **figer** la 1re ligne
- Écrire des **formules** avec références relatives et absolues
- Utiliser les fonctions de base : **SOMME**, **MOYENNE**, **MIN** / **MAX**, **NB** / **NBVAL**
- Trier et filtrer sans casser le tableau

---

## À quoi sert Google Sheets ?

**Google Sheets** = tableur **en ligne**, fichier dans **Drive**.

- Calculs et tableaux sans installer Excel
- Travail à plusieurs sur le **même** fichier
- Historique des versions (rappel séances 2 et 3)

Utile en ingénierie : relevés de mesures, bilans, plannings chiffrés, listes de matériel, petits jeux de données.

Excel reste possible : on peut **importer** / **exporter** `.xlsx`. Pour collaborer, préférez le Sheet natif.

---

## Interface utile

Zones à connaître :

1. **Grille** : cellules adressées (A1, B2…)
2. **Onglets** en bas : plusieurs **feuilles** dans le même fichier
3. **Barre de formules** (sous les menus) : contenu exact de la cellule active
4. **Barre d’outils** : format nombre, gras, bordures, alignement…

Cliquez une cellule pour la sélectionner ; la barre de formules montre ce qui est vraiment stocké (valeur ou formule).

---

## Types de données

Sheets interprète ce que vous tapez :

| Type | Exemples | Remarque |
| --- | --- | --- |
| **Texte** | `Pompe P1`, `OK` | Aligné à gauche par défaut |
| **Nombre** | `12`, `3,14`, `-5` | Calculable ; séparateur décimal selon la locale |
| **Date** / heure | `18/10/2026`, `14:30` | Stockées comme nombres ; format d’affichage à part |

Attention : un « nombre » tapé avec une apostrophe (`'12`) ou collé comme texte **ne se calcule pas**. La cellule reste à gauche, souvent signe d’un texte.

---

## Mise en forme

Menu **Format** (ou barre d’outils) :

- **Nombre** : décimales, pourcentages, devise, date
- **Alignement** : horizontal / vertical ; en-têtes souvent centrés
- **Bordures** et **couleur** de fond : lisibilité, pas décoration
- **Figer** : **Affichage** → **Figer** → **1 ligne** (les en-têtes restent visibles en scrollant)

Une colonne de mesures : même format (ex. 2 décimales) sur toute la plage.

---

## Tableau propre

Un bon tableau se lit et se **filtre** sans surprise.

| Faire | Éviter |
| --- | --- |
| **1re ligne** = en-têtes clairs | Titre fusionné à la place des en-têtes |
| **1 ligne = 1 enregistrement** | Plusieurs infos dans la même cellule |
| Une colonne = une grandeur | Colonnes vides « pour aérer » |
| Plage continue, sans lignes vides au milieu | **Fusions** inutiles qui cassent tri / formules |

Les fusions : réservez-les aux titres hors zone de données, pas au cœur du tableau.

---

## Références : cellules et plages

Adresse **A1** : colonne lettre + ligne numéro.

| Notation | Signifie |
| --- | --- |
| `B3` | Une cellule |
| `A2:A20` | Une **plage** (colonne A, lignes 2 à 20) |
| `A2:C10` | Un **bloc** rectangulaire |
| `Feuille2!B3` | Cellule B3 de l’onglet nommé `Feuille2` |

Sélectionnez une plage à la souris pendant que vous écrivez la formule : Sheets remplit la référence.

---

## Formules : `=` et opérateurs

Toute formule **commence par** `=`.

Opérateurs courants :

| Opérateur | Rôle | Exemple |
| --- | --- | --- |
| `+` `-` `*` `/` | Calcul | `=B2*C2` |
| `()` | Priorité | `=(A1+A2)/2` |
| `&` | Coller du texte | `="Mesure "&A1` |

Après Entrée, la cellule **affiche le résultat** ; la barre de formules montre encore la formule.

Erreur fréquente : oublier le `=` (Sheets traite alors le texte comme du libellé).

---

## Fonctions de base

Syntaxe : `=NOM(plage_ou_arguments)`.

| Fonction | Rôle | Exemple |
| --- | --- | --- |
| **SOMME** | Additionne | `=SOMME(B2:B20)` |
| **MOYENNE** | Moyenne | `=MOYENNE(B2:B20)` |
| **MIN** / **MAX** | Extrêmes | `=MAX(C2:C20)` |
| **NB** | Compte les **nombres** | `=NB(B2:B20)` |
| **NBVAL** | Compte les cellules **non vides** | `=NBVAL(A2:A20)` |

Aide en cours de saisie : après `=SOM`, Sheets propose la fonction ; Tab pour valider.

---

## Relatif vs absolu (`$`)

Quand on **recopie** une formule :

| Type | Écriture | Au déplacement |
| --- | --- | --- |
| **Relatif** | `B2` | Suit la nouvelle ligne / colonne |
| **Absolu** | `$B$2` | Reste bloqué sur B2 |
| Mixte | `$B2` ou `B$2` | Bloque seulement la colonne ou la ligne |

Exemple : TVA fixe en `$E$1`, montants en colonne B → `=B2*$E$1`, puis recopier vers le bas.

Sans `$`, la référence « glisse » et le calcul devient faux.

---

## Poignée de recopie

Petit carré en bas à droite de la sélection : la **poignée de recopie**.

- Tirez vers le bas / la droite pour étendre une formule
- Les références **relatives** s’ajustent ; les **`$`** restent fixes
- Double-clic sur la poignée : remplit souvent jusqu’à la fin de la colonne voisine

Contrôlez 2 ou 3 cellules après copie : résultat + formule dans la barre.

---

## Tris et filtres (aperçu)

Sur un tableau avec en-têtes :

1. Sélectionnez la plage (ou une cellule dedans)
2. **Données** → **Créer un filtre** (icônes dans les en-têtes)
3. Filtrer : n’afficher que certaines valeurs ; **trier** A→Z ou par nombre

Le filtre masque des lignes, il ne les efface pas. Désactivez le filtre pour revoir tout le jeu.

S5 ira plus loin (validation, mise en forme conditionnelle, graphiques).

---

## Erreurs fréquentes

| Affichage | Cause typique | Piste |
| --- | --- | --- |
| `#DIV/0!` | Division par zéro (ou cellule vide traitée comme 0) | Vérifier le dénominateur |
| `#REF!` | Référence vers une cellule **supprimée** | Réécrire la formule |
| `#VALUE!` / résultat bizarre | **Texte** là où un nombre est attendu | Typer / reformater en nombre |
| Formule affichée telle quelle | Oubli du `=` ou cellule en format texte | Corriger et valider |

Astuce : alignez une colonne « nombres » : si tout n’est pas à droite, cherchez les textes déguisés.

---

## Bonnes pratiques

1. Une **feuille** = un sujet clair ; nommez les onglets
2. En-têtes en **ligne 1**, données en dessous, **sans** fusion dans la zone utile
3. Formules plutôt que calculatrices à côté : le fichier reste à jour
4. **`$`** dès qu’une cellule doit rester fixe à la recopie
5. Même **format nombre** sur toute une colonne de mesures
6. Figer la **1re ligne** dès que le tableau dépasse l’écran
7. Fichier dans le **dossier Drive** du projet, nommé clairement

---

## Tâches évaluées

**TBA**

→ [Tâches évaluées](taches_seance_04.html)

---

## Deadline

**Deadline : la veille de la prochaine séance, 20:00**

→ [Tâches évaluées](taches_seance_04.html)
