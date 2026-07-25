# 0005 — Structure par chantiers

- **Date** : 2026-07-25
- **Statut** : adoptée
- **Adoptée le** : 2026-07-25
- **Décideurs** : y-magma (via validation explicite « Ok pour option B »)
- **Sources** : [`../syntheses/2026-07-25-critique-structure-du-cerveau.md`](../syntheses/2026-07-25-critique-structure-du-cerveau.md), [`../idees/2026-07-25-structure-par-chantiers.md`](../idees/2026-07-25-structure-par-chantiers.md)

## Contexte

Le pipeline en 5 dossiers (`idees/` → … → `decisions/`) ouvre plus de boucles qu'il n'en ferme. Besoin d'un lieu unique par sujet.

## Options envisagées

1. **A — Alléger le pipeline** — moins de friction, même découpe.
2. **B — Chantiers** — un dossier = un sujet (`seed` / `debate` / `map` / `formula`).
3. **C/D/E** — wiki plat / IBIS / Pol.is-first (reportés).

## Décision

**Option B.** Nouveau foyer primaire : [`../chantiers/`](../chantiers/).  
`decisions/`, `vision/`, `slogans/noyau/` restent transverses.  
Anciens dossiers d'étape = **legacy** (liens + migration progressive), plus le lieu d'écriture par défaut.

## Conséquences

- **Positives** : un sujet = un lieu ; trou visible si `map.md` manque ; aligné « fermer des boucles ».
- **Négatives / coûts** : migration ; liens cassés à réparer ; dual temporaire.
- **À revisiter si** : les chantiers redeviennent des mini-pipelines bureaucratiques, ou si un graphe IBIS s'impose.
