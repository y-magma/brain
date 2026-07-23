# Décisions

Le **journal des choix structurants** (forme de l'outil, orientations, conventions). Format ADR léger (*Architecture/Any Decision Record*).

## Consigner une décision

1. Copier [`_gabarit-decision.md`](_gabarit-decision.md).
2. Renommer en `NNNN-titre.md` (numéro croissant, ex. `0001-langue-de-travail.md`).
3. Remplir, ouvrir une Pull Request.

## Principe

Une décision n'efface pas les alternatives : elle les consigne, avec le contexte et les conséquences. Si on change d'avis plus tard, on écrit une **nouvelle** décision qui remplace l'ancienne (statut `remplacée par …`) — on ne réécrit pas l'histoire. **La décision appartient aux humains** ; l'IA n'en rédige que le brouillon.
