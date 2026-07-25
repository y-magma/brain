# Chantiers

> **Un sujet = un lieu.** On ferme des boucles, on n’ouvre pas des dossiers pour le sport.
>
> Décision : [`../decisions/0005-structure-par-chantiers.md`](../decisions/0005-structure-par-chantiers.md)

![Quatre portes-dossiers sur un chemin — métaphore des chantiers](../assets/illustrations/chantiers-portes.jpg)

*Quatre portes. Un chemin. Choisis un chantier, pas une étape administrative.*

## Anatomie d'un chantier

| Fichier | Rôle | Signal |
|---------|------|--------|
| `seed.md` | Graine + slogan | « Pourquoi on touche à ça » |
| `debate.md` | Steelman pour / contre | « On a vraiment écouté l’autre camp » |
| `map.md` | Convergences / divergences / angles morts | **Pas de map = boucle ouverte** |
| `formula.md` | Formule(s) + raisonnement | « Ce qu’on peut répéter sans mentir » |

Optionnel : `notes.md`, illustrations dans le dossier ou dans `assets/illustrations/`.

## Créer un chantier

1. Copier la structure (voir un pilote ci-dessous).
2. Nommer en kebab-case : `chantiers/mon-sujet/`.
3. Remplir `seed.md` **avant** le reste.
4. Ouvrir une PR. Mettre à jour [`../CARTE.md`](../CARTE.md) + sidebar.

## Index actif

| Chantier | Slogan | Boucle | Lien |
|----------|--------|--------|------|
| Structure du cerveau | « Fermer des boucles, pas ouvrir des dossiers. » | map ✓ | [ouvrir](structure-cerveau/) |
| Atlas des slogans | « Machine à ralentir les slogans sans les tuer » | map ✗ | [ouvrir](atlas-slogans/) |
| Simplicité | « Dsl, j'ai pas eu le temps de faire simple. » | map ~ | [ouvrir](simplicite/) |
| Ton empêcheur | « Empêcheur de tourner en rond — titiller, pas cliquer. » | map ~ | [ouvrir](ton-empecheur/) |

## Transversal (hors chantier)

- [`../decisions/`](../decisions/) — ADR
- [`../vision/`](../vision/) — manifeste, glossaire
- [`../slogans/noyau/`](../slogans/noyau/) — axiomes du collectif
- [`../archive/`](../archive/) — hors circuit

## Legacy

`idees/`, `points-de-vue/`, `syntheses/` : **plus le lieu d’écriture par défaut**. Fichiers migrés → stubs qui pointent ici. Migration progressive du reste.
