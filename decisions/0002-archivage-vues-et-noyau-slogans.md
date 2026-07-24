# 0002 — Archivage, vues par étape, et noyau de slogans

- **Date** : 2026-07-24
- **Statut** : adoptée
- **Adoptée le** : 2026-07-24
- **Décideurs** : y-magma, Vincent
- **Sources** : [`../archive/README.md`](../archive/README.md), [`../slogans/noyau/README.md`](../slogans/noyau/README.md), [`../idees/2026-07-24-noyau-axiomes-de-slogans.md`](../idees/2026-07-24-noyau-axiomes-de-slogans.md), [`../CARTE.md`](../CARTE.md)

## Contexte

Le dépôt grossit : beaucoup de graines dans `idees/`, une sidebar qui liste tout au même niveau, une Carte dense. Besoins exprimés :

1. **Archiver** sans effacer ce qu'on ne veut plus pousser.
2. **Voir séparément** idées / points de vue / synthèses / slogans / décisions (sur le site comme dans Git).
3. Traiter les **slogans** comme couche cruciale : chaque idée devrait pouvoir se dire en formule ; viser un **noyau minimal d'axiomes**, enrichissable en multi-échelle / multi-granularité.

## Options envisagées

### A. Archivage

1. **Dossier `archive/` miroir** (sous-dossiers par étape) — navigation claire ; déplacement explicite.
2. **Statut `archivée` sans déplacement** — simple, mais la Carte et les index restent bruyants.
3. **Branches / tags Git seulement** — fidèle à Git, peu lisible pour un humain non technique.

### B. Navigation web

1. **Sidebar groupée par dossier d'étape** + README index riches — pas de nouveau outil.
2. **Sous-sites / pages cover Docsify** — plus joli, plus de config.
3. **Ne rien changer** — laisser la liste plate « contributions en cours ».

### C. Slogans / noyau

1. **`slogans/noyau/`** = axiomes adoptés du collectif ; `slogans/` = dérivés / candidats ; chaque idée porte un *slogan candidat* dès la graine.
2. **Un seul dossier plat** avec un label `noyau` dans le front-matter Markdown.
3. **Reporter** jusqu'à ce qu'une synthèse existe (cycle strict actuel) — plus sûr anti-populisme, plus lent à rendre les slogans visibles.

## Décision

- **Archivage** : option A.1 — dossier [`../archive/`](../archive/) miroir, procédure dans son README.
- **Navigation** : option B.1 — sidebar et README **par étape** ; la Carte montre les *grands sujets* et *comment avancer*, pas la liste exhaustive.
- **Slogans** : option C.1 — instaurer un **noyau** ; autoriser un *slogan candidat* dès l'idée (hypothèse de travail, pas axiome adopté) ; enrichir gabarits (échelle, granularité). Le garde-fou reste : pas de formule orpheline de raisonnement.

> Tranché le 2026-07-24 : la structure est déjà en place et utilisée (premier passage d'archivage des graines hors vision produit).

## Conséquences

- **Positives** : dépôt plus lisible ; archive sans perte ; les slogans deviennent visibles tôt sans être confondus avec des vérités adoptées ; le site reflète enfin la structure des dossiers.
- **Négatives / coûts** : discipline de déplacement + mise à jour Carte/sidebar à chaque archive ; risque de confondre *slogan candidat* (idée) et *axiome du noyau* (adopté) — à nommer explicitement dans le glossaire.
- **À revisiter si** : le noyau grossit sans critères d'admission ; l'archive devient un fourre-tout non motivé ; la sidebar redevient une liste plate.
