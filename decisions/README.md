# Décisions

Le **journal des choix structurants** (forme de l'outil, orientations, conventions). Format ADR léger (*Architecture/Any Decision Record*).

## Consigner une décision

1. Copier [`_gabarit-decision.md`](_gabarit-decision.md).
2. Renommer en `NNNN-titre.md` (numéro croissant, ex. `0001-langue-de-travail.md`).
3. Remplir, ouvrir une Pull Request.

## Principe

Une décision n'efface pas les alternatives : elle les consigne, avec le contexte et les conséquences. Si on change d'avis plus tard, on écrit une **nouvelle** décision qui remplace l'ancienne (statut `remplacée par …`) — on ne réécrit pas l'histoire. Les décisions remplacées peuvent rejoindre [`../archive/decisions/`](../archive/decisions/). **La décision appartient aux humains** ; l'IA n'en rédige que le brouillon.

Les décisions **adoptées** restent ici (visibles) — on n'archive que celles qui sont *remplacées*.

## Index

| # | Décision | Statut | Lien |
|---|----------|--------|------|
| 0001 | Langue (français) et méthode (cycle en 5 temps) | **adoptée** | [ouvrir](0001-langue-et-methode-de-travail.md) |
| 0002 | Archivage, vues par étape, noyau de slogans | **adoptée** | [ouvrir](0002-archivage-vues-et-noyau-slogans.md) |
| 0003 | Slogans = brique majeure ; accroche obligatoire des idées | **proposée** | [ouvrir](0003-slogans-brique-et-accroche-des-idees.md) |
