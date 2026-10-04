---
marp: true
theme: outils-info-ia
title: "Séance 3 — Google Docs"
paginate: true
header: "Outils Info & IA — Séance 3 [Sylvain Huraux - HE2B - ISIB](mailto:shuraux@he2b.be)"
footer: "[← Retour à l'accueil](../../index.html)"
---

## Séance 3

Google Docs

---

## Objectifs de la séance

- Créer un **Google Doc** au bon endroit dans Drive
- Structurer avec des **styles** (titres), pas du gras manuel
- Ajouter **table des matières**, **en-tête**, **numéros de page**, **figures**
- Collaborer : **commentaires** et **mode suggestion**
- Exporter un **PDF** lisible (sauts de page, sommaire)

---

## À quoi sert Google Docs ?

**Google Docs** = traitement de texte **en ligne**, fichier dans **Drive**.

- Un seul document, pas dix copies `v3_final.docx`
- Travail à plusieurs en même temps
- Historique des versions (rappel séance 2)

Utile pour : compte-rendu, note technique, cahier des charges, rapport.

Word reste possible : on peut **importer** / **exporter** `.docx`. Pour collaborer, préférez le Doc natif.

---

## Créer au bon endroit

Depuis **Drive**, bouton **Nouveau** → **Google Docs**.

- Créez le fichier **dans le dossier** du projet (évite « Documents sans titre » à la racine)
- Nommez tout de suite : `AAAA-MM-JJ_Projet_description`
- Un Doc « orphelin » se retrouve souvent dans *Récents*, pas dans votre arborescence

Rappel S2 : le fichier vit dans Drive ; le lien + les **droits** valent mieux qu’une PJ.

---

## Interface utile

Zones à connaître :

1. **Barre de menus** : Fichier, Édition, Insertion, Format…
2. **Barre d’outils** : gras, listes, liens (raccourcis du quotidien)
3. **Plan du document** (*outline*, à gauche) : titres cliquables
4. **Mode** : modification / suggestion / lecture

Affichez le plan : **Affichage** → **Afficher le plan du document**.

---

## Styles de titres (pas du gras)

Un titre, c’est un **style** : *Titre 1*, *Titre 2*, *Titre 3*, *Texte normal*.

| Faire | Éviter |
| --- | --- |
| Appliquer **Titre 1** / **Titre 2** | Gros gras + souligné « à la main » |
| Hiérarchie réelle (1 puis 2) | Tout en Titre 1 |
| Texte du corps en *Normal* | Titres pour aérer un paragraphe |

Les styles alimentent le **plan** et la **table des matières**. Sans eux, le document n’a pas de structure machine.

---

## Plan et table des matières

Si les titres sont des styles :

1. le **plan** à gauche sert de navigation
2. **Insertion** → **Table des matières** : sommaire **automatique**
3. après une grosse coupe : clic sur la TdM → **mettre à jour**

Une TdM tapée à la main se casse au premier ajout de section.

Pour un livrable paginé : mode **Pages** (pas « sans pages »), sinon le PDF n’a pas de vrai saut de page.

---

## En-tête, pied de page, numéros

**Insertion** → **En-tête** / **Pied de page** / **Numéros de page**.

En pratique :

- En-tête : nom du document ou du projet (court)
- Pied : **numéro de page** (souvent centré ou à droite)
- Option : première page **différente** (page de garde sans numéro)

Vérifiez en **aperçu d’impression** avant d’exporter.

---

## Page de garde

Première page = identité du livrable, pas le début du texte.

À faire figurer, selon le contexte :

- **Titre** du document
- **Auteurs** / équipe
- **Date**
- Destinataire, projet ou référence

Laissez le corps commencer **après** (saut de page). Le titre de garde n’est pas forcément un *Titre 1* du plan.

---

## Images et légendes

**Insertion** → **Image** (Drive, upload, URL).

- Une image **lisible** une fois imprimée (pas une capture minuscule)
- **Légende** juste en dessous : `Figure 1 : …`
- Ancrez l’image au texte (évite qu’elle flotte toute seule)

Une figure sans légende n’est pas citée dans un rapport.

---

## Commentaires

Un **commentaire** porte sur un passage (sélection → icône commentaire, ou `Ctrl`+`Alt`+`M`).

- Écrire une **demande actionnable** (« préciser la date », pas « ok »)
- **@nom** pour notifier quelqu’un
- **Résoudre** le fil une fois traité (il reste dans l’historique)

Commenter ≠ réécrire le texte à la place de l’auteur.

---

## Mode suggestion

Trois modes en haut à droite :

| Mode | Effet |
| --- | --- |
| **Modification** | On écrit directement dans le texte |
| **Suggestion** | Les changements apparaissent comme des **propositions** (accepter / refuser) |
| **Lecture** | On lit, on ne casse rien |

Pour une relecture : **suggestion** (ou commentateur au partage). Pour rédiger à deux : **modification**, avec un accord sur qui touche à quoi.

---

## Partage : rappel séance 2

Les droits s’appliquent aussi au Doc :

| Rôle | Pour… |
| --- | --- |
| **Lecteur** | Consulter / souvent exporter |
| **Commentateur** | Relire sans réécrire |
| **Éditeur** | Rédiger ensemble |

Le dossier peut donner un droit **héritage** ; on peut **monter** le rôle sur un fichier (ex. lecteur sur le dossier, éditeur sur ce Doc).

Vérifier **qui peut ouvrir** avant d’envoyer le lien.

---

## Historique des versions

**Fichier** → **Historique des versions** → Voir l’historique.

- Retrouver une version d’hier
- Voir **qui** a modifié quoi
- **Nommer** un jalon (ex. `Avant relecture`)

Mieux qu’un `rapport_final2.docx` en pièce jointe.

---

## Exporter en PDF

**Fichier** → **Télécharger** → **PDF**.

Contrôler dans le PDF :

- table des matières à jour
- sauts de page (titre seul en bas de page = à corriger)
- figures lisibles, légendes collées à l’image
- en-tête / numéros présents

Le PDF est un **instantané** pour remise ou archive. Le Doc Drive reste la version de travail.

---

## Bonnes pratiques (contexte pro)

1. Un Doc **dans le dossier** du projet, nommé clairement
2. **Styles** de titres dès la première section
3. TdM auto + en-tête / numéros **avant** la relecture finale
4. Relecture : **commentaires** ou **suggestions**, pas un second fichier
5. Droits **minimum** (relecture ≠ édition)
6. PDF de remise **après** mise à jour de la TdM

---

## Erreurs fréquentes

- Titres en gras manuel → pas de plan, pas de TdM fiable
- Tout le monde **éditeur** « au cas où »
- Figure sans légende, ou illisible une fois imprimée
- Exporter le PDF **avant** d’avoir mis à jour le sommaire
- Copier le Doc pour chaque relecteur (les versions divergent)

---

## Tâche 1 — Mini-rapport structuré

Créez un Google Doc nommé :

`AAAA-MM-JJ_OutilsInformatiques_Nom_minirapport`

À vérifier : page de garde, **styles** Titre 1 / Titre 2, **TdM** auto, intro, **figure** + légende, en-tête et **numéros de page**.

→ [Tâches évaluées](taches_seance_03.html)

---

## Tâche 2 — Collaboration

Sur ce Doc :

1. partage adapté (**éditeur** ou **commentateur**)
2. **2 commentaires** actionnables (pas « ok »)
3. **1 suggestion** de reformulation
4. **résoudre** un fil une fois traité

→ [Tâches évaluées](taches_seance_03.html)

---

## Tâche 3 — Remise PDF

1. Téléchargez le Doc en **PDF** (nom parallèle au Doc)
2. Déposez-le dans votre dossier Drive de travail
3. Contrôlez sommaire, sauts de page, lisibilité de la figure

→ [Tâches évaluées](taches_seance_03.html)

---

## Deadline

Réalisation des tâches : **au plus tard la veille de la prochaine séance, à 20:00**.

→ [Tâches évaluées](taches_seance_03.html)
