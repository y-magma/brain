# Le processus

> Depuis [0005](../decisions/0005-structure-par-chantiers.md) : on travaille par **chantiers**, pas par pipeline de dossiers.

```
   chantiers/<sujet>/
     seed.md ──▶ debate.md ──▶ map.md ──▶ formula.md
         ▲                         │
         └──── rouvrir / itérer ◀──┘

   decisions/     ← transverse (ADR)
   slogans/noyau/ ← axiomes du collectif
   vision/        ← manifeste, glossaire
```

## 1. Ouvrir ou rejoindre un chantier — `chantiers/`

- Un sujet = un dossier kebab-case.
- Remplir `seed.md` d’abord (slogan obligatoire).
- Ton : [`ton.md`](ton.md) — fun, tranchant, anti-pute-à-clic.

## 2. Confronter — `debate.md`

Steelman pour **et** contre. Positions absentes bienvenues.  
L’IA propose les camps oubliés ; l’humain corrige.

## 3. Cartographier — `map.md`

Convergences / divergences / angles morts. Multi-échelle.  
**Pas de map = boucle ouverte** (c’est voulu, c’est visible).

## 4. Distiller — `formula.md` (+ noyau)

Formule + raisonnement. Candidature noyau si boussole collective.

## 5. Trancher — `decisions/`

ADR léger. L’IA brouillonne ; **l’humain décide**.

## 6. Archiver

Déplacer le dossier chantier entier vers `archive/chantiers/` (à créer au besoin) + motif.

## Pull Request

Toujours. Relecture humaine = règles de fond + ton (pas de clickbait, steelman présent).

## Legacy

`idees/`, `points-de-vue/`, `syntheses/` : stubs / files en migration. **N’y écris plus** sauf redirection.
