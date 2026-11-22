# Séance 5 — Google Sheets (2) + Forms

<nav class="page-nav">
  <a href="../../index.html">Accueil</a>
  <a href="cours_seance_05.html">Slides</a>
  <a href="taches_seance_05.html">Tâches</a>
</nav>

## Objectifs de la séance

- Contrôler la saisie avec la **validation de données** (liste, nombre)
- Relire un tableau avec **filtres** et un repère visuel (mise en forme conditionnelle)
- Créer un **graphique** lisible : type adapté, titres, légende
- Créer un **Google Form** (types utiles BA1) et le **lier** à une feuille
- Partager le formulaire et lire les réponses dans Sheets
- Enchaîner mentalement : **Forms → Sheets → graphique**

## Rappel express S4

Déjà vu, on ne refait pas :

- Tableau propre, types, mise en forme, **figer** la 1re ligne
- Références A1, plages, feuilles, formules `=` et opérateurs
- **SOMME**, **MOYENNE**, **MIN** / **MAX**, **NB** / **NBVAL**
- Relatif vs `$`, poignée de recopie
- Tris / filtres en **aperçu**

Aujourd’hui : filtres en pratique, validation, MFC légère, graphiques, puis Forms.

## Filtres : afficher sans effacer

Sur un tableau avec en-têtes en ligne 1 :

1. Une cellule dans la plage → **Données** → **Créer un filtre**
2. Icônes dans les en-têtes : cocher / décocher des valeurs
3. Filtrer sur **1 ou 2 colonnes**, trier A→Z ou par nombre dans le menu du filtre

Le filtre **masque** des lignes, il ne les **efface** pas.

Désactiver : **Données** → **Supprimer le filtre** (tout réapparaît).

Erreur fréquente : filtrer une plage sans vraie ligne d’en-têtes → résultats incohérents.

## Validation de données : pourquoi

Sans contrôle, n’importe qui tape n’importe quoi : `oui` / `Oui` / `OK` / `1`.

La **validation** limite ce qu’on peut saisir dans une cellule ou une colonne.

- Moins d’erreurs de frappe
- Listes homogènes (filtrables, graphiquables)
- Messages clairs si la saisie est refusée

Menu : sélectionner la plage → **Données** → **Validation des données**.

## Validation : listes et nombres

Deux cas utiles en BA1 :

| Critère | Exemple | Effet |
| --- | --- | --- |
| **Liste d’éléments** | `OK, KO, N/A` | Liste déroulante |
| **Nombre** | entre `0` et `100` | Refuse hors plage |

Réglages à cocher souvent :

- **Refuser la saisie** (pas seulement un avertissement)
- Afficher un **texte d’aide** court sur la cellule

Erreur fréquente : valider seulement la 1re ligne de données. Étendez la plage (ou une colonne entière hors en-tête).

## Mise en forme conditionnelle (aperçu)

Repère **visuel** : la cellule change selon une règle, sans formule obligatoire.

1. Sélectionner la plage
2. **Format** → **Mise en forme conditionnelle**
3. Une règle simple, par ex. :
   - **Valeur de cellule** > un seuil
   - **Le texte contient** un mot (`KO`, `retard`…)

Couleur de fond ou de texte : un signal, pas un arc-en-ciel.

Une règle suffit pour démarrer. Trop de règles = tableau illisible.

## Graphiques : choisir le bon type

Sélectionner la plage (en-têtes inclus) → **Insertion** → **Graphique**.

| Type | Quand |
| --- | --- |
| **Barres** / colonnes | Comparer des catégories |
| **Lignes** | Évolution dans le temps |
| **Secteurs** (camembert) | Parts d’un **tout** (peu de parts) |

Le type se change dans l’éditeur de graphique (à droite).

Données sales (textes dans une colonne de nombres, lignes vides) → graphique absurde. Nettoyez d’abord.

## Graphiques : titres, axes, légende

Dans l’éditeur de graphique :

- **Titre** du graphique : ce que l’on compare (pas « Graphique 1 »)
- **Axes** : libellés si besoin (unité, grandeur)
- **Légende** : utile dès qu’il y a plusieurs séries

Placez le graphique sur la feuille (déplacer / redimensionner).

Lisibilité : assez grand pour se lire sans zoom extrême, une idée par graphique.

## Google Forms : à quoi ça sert

**Google Forms** = questionnaire en ligne. Les réponses peuvent alimenter un **Sheets**.

- Collecte structurée (pas un fil de mails)
- Types de questions prêts à l’emploi
- Lien direct vers une feuille de réponses

Utile : retour de labo, inscription, sondage court, checklist.

Hors séance : quiz noté complexe, branchements longs, add-ons.

## Créer un formulaire et types

Création : [forms.google.com](https://forms.google.com) ou Drive → **Nouveau** → **Google Forms**.

- Titre + **description** courte
- Ajouter des questions, choisir le **type**

Types utiles BA1 :

| Type | Usage |
| --- | --- |
| **Choix multiples** | Une seule réponse parmi plusieurs |
| **Cases à cocher** | Plusieurs réponses possibles |
| **Liste déroulante** | Même idée, liste compacte |
| **Réponse courte** / **paragraphe** | Texte libre |
| **Nombre** / **échelle** | Quantité ou note subjective |

## Réglages utiles

Sur une question :

- Case **Obligatoire** : pas d’envoi sans réponse

Dans **Paramètres** (engrenage) :

- **Collecter les adresses e-mail** : oui / non (selon le besoin)
- **Limiter à une réponse** : compte Google requis
- Qui peut répondre : comptes du domaine vs **tout le monde** (lien)

Ordre des questions : glisser-déposer, numérotation auto.

Erreur fréquente : oublier « obligatoire » sur la question clé, puis des lignes vides dans Sheets.

## Lier les réponses à Sheets

Dans le Form : onglet **Réponses** → icône Sheets **Sélectionner la destination des réponses**.

Deux options :

1. **Créer une nouvelle feuille de calcul** (nouveau fichier Drive)
2. **Sélectionner une feuille de calcul existante** (ajoute un onglet dans un classeur déjà là)

Colonnes = questions. Première colonne souvent un **horodatage**.

Préférez lier à un fichier que vous maîtrisez déjà, plutôt qu’empiler des tableurs orphelins.

## Partager le formulaire (lien)

Bouton **Envoyer** (haut à droite) :

- Onglet **lien** : copier l’URL à coller (mail, Chat, Drive…)
- Raccourcir le lien si proposé

Qui répond :

- Lien ouvert (« tout le monde ») : pratique en salle
- Restriction au compte HE2B : plus de contrôle, compte requis

Le Form et le Sheet lié ont des **droits séparés** : partager le Form pour répondre ≠ donner l’édition du Sheet.

## Lire sans casser la feuille Réponses

Deux vues :

1. Onglet **Réponses** dans Forms : résumé, graphiques auto
2. Feuille liée dans Sheets : une ligne = une réponse

À faire :

- Filtrer / trier, recopier vers une feuille **Analyse** pour vos calculs
- Ajouter validation ou MFC sur une feuille à part si besoin

À éviter :

- Renommer / supprimer / réordonner à la main les colonnes **auto** du Form
- Éditer les cellules de réponses comme un brouillon (casse le lien mental Form ↔ Sheet)

## Chaîne Forms → Sheets → graphique

Enchaînement type :

1. **Form** : questions claires, types adaptés, obligatoires utiles
2. **Sheets** : feuille de réponses (horodatage + colonnes)
3. **Propreté** : filtres, validation ailleurs si besoin, MFC légère
4. **Graphique** : type adapté + titre, sur une plage propre

Objectif de fin de module Sheets/Forms : collecter → stocker → visualiser, dans le même écosystème Drive.

## Tâches évaluées

**TBA**

[Tâches évaluées](taches_seance_05.html)

## Deadline

**Deadline : la veille de la prochaine séance, 20:00**

[Tâches évaluées](taches_seance_05.html)

<nav class="page-nav">
  <a href="../../index.html">Accueil</a>
  <a href="cours_seance_05.html">Slides</a>
  <a href="taches_seance_05.html">Tâches</a>
</nav>

<footer class="site-footer"><a href="mailto:shuraux@he2b.be">Sylvain Huraux - HE2B - ISIB</a></footer>
