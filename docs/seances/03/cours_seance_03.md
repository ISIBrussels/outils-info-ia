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
- Nommez tout de suite : cliquez le **titre en haut à gauche** du Doc (pas besoin de passer par Drive) — ex. `AAAA-MM-JJ_Projet_description`
- Un Doc « orphelin » se retrouve souvent dans *Récents*, pas dans votre arborescence

Rappel S2 : le fichier vit dans Drive ; le lien + les **droits** valent mieux qu’une PJ.

---

## Interface utile

Zones à connaître :

1. **Barre de menus** : Fichier, Édition, Insertion, Format…
2. **Barre d’outils** : gras, listes, liens (raccourcis du quotidien)
3. **Onglets et plan** (icône en haut à gauche) : titres cliquables + onglets du Doc
4. **Mode** : modification / suggestion / lecture

Affichez-les via l’icône **Afficher les onglets et le plan** (haut à gauche). Les **onglets** d’un Doc jouent un rôle proche des **feuilles** dans Sheets : plusieurs sections dans le même fichier.

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

Google Docs **n’a pas** de menu Word du type *Insertion → Page de garde* avec modèles prêts. On la construit sur la **1re page** du Doc.

À y mettre, selon le contexte : **titre**, **auteurs** / équipe, **date**, destinataire ou projet. Éventuellement un logo : **Insertion** → **Image**.

Ensuite : **Insertion** → **Saut** → **Saut de page** pour que le corps commence page 2. Le titre de garde n’est pas forcément un *Titre 1* du plan.

Numéros : **Insertion** → **Éléments de page** → **Numéro de page** (options pour démarrer après la page de garde / première page différente).

---

## Menus Insertion et Format

Deux menus à connaître tôt :

| Menu | Sert surtout à… |
| --- | --- |
| **Insertion** | Ajouter : **image**, **saut** de page, **tableau**, **table des matières**, **éléments de page** (en-tête, pied, numéros)… |
| **Format** | Soigner le texte : **styles**, alignement, interligne, options de **liste**… |

La barre d’outils reprend les actions du quotidien ; les menus donnent le reste.

---

## Listes

Dans la **barre d’outils** (ou **Format**) :

- **Puces** : sans ordre imposé — **numérotées** : 1, 2, 3… (évitez de taper `1.` / `-` à la main)
- **Tab** / **Maj**+**Tab** (ou indent) : descendre / remonter d’un **niveau** dans la liste

Idée BA1 : **lier niveau de titre ↔ niveau de liste** — *Titre 1* → items niveau 1 ; *Titre 2* → sous-liste ; etc. Même hiérarchie partout.

---

## Saut de page

Un **saut de page** force le texte suivant à commencer sur une **nouvelle page** : **Insertion** → **Saut** → **Saut de page**.

| Faire | Éviter |
| --- | --- |
| Un vrai saut (page de garde → corps, nouvelle section…) | Enchaîner des **Entrée** pour « arriver » sur la page suivante |
| Reste stable si on modifie le texte au-dessus | Se casse dès qu’on ajoute ou coupe du contenu plus haut |

---

## Images et légendes

**Insertion** → **Image** (Drive, upload, URL).

- Une image **lisible** une fois imprimée (pas une capture minuscule)
- **Légende** juste en dessous : `Figure 1 : …`
- Ancrez l’image au texte (évite qu’elle flotte toute seule)

Une figure sans légende n’est pas citée dans un rapport.

---

## Commentaires

Un **commentaire** porte sur un passage (sélection → bouton **Commentaire** en **haut à gauche** de l’interface Docs, ou `Ctrl`+`Alt`+`M`).

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

## Bonnes pratiques

1. Un Doc **dans le dossier** du projet, nommé clairement
2. **Styles** de titres dès la première section
3. **Saut de page** réel (pas des Entrée) pour séparer page de garde / corps
4. TdM auto + en-tête / numéros **avant** la relecture finale
5. Relecture : **commentaires** ou **suggestions**, pas un second fichier
6. Droits **minimum** (relecture ≠ édition)
7. PDF de remise **après** mise à jour de la TdM

---

## Tâche — Remplir le Doc partagé (3 points)

Sur le **Doc S2** : nom `YYYY-MM-DD_…` ; page de garde **Outils Info & IA** / **Rapport de travail** ; en-tête `Outils Info & IA - Rapport` ; pied = n° de page + nom ; styles, listes, TdM, figure, commentaires + suggestion, **PDF**.

→ [Tâches évaluées](taches_seance_03.html)

---

## Deadline

**Deadline : la veille de la prochaine séance, 20:00**

→ [Tâches évaluées](taches_seance_03.html)
