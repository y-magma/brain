# brain

**Un atelier collaboratif humain + IA pour penser, confronter et faire émerger des idées — ensemble.**

`brain` n'est pas (encore) un logiciel. C'est un espace de travail sur GitHub, à la manière d'un « wiki-LLM », où l'on brainstorme et où l'on avance concrètement sur des idées **toujours en mouvement**. On y explore la forme — **encore inconnue** — que pourrait prendre une machine à penser / un outil de démocratie. Les slogans et expressions courtes y jouent un **grand rôle** (accroche de chaque idée, matériau, distillation), sans définir à eux seuls le projet.

## Pourquoi

- Sortir des slogans creux et du populisme, sans renoncer aux **idées fortes et mémorables**.
- Retrouver le goût de **discuter avec un point de vue opposé**.
- Cartographier honnêtement les **convergences** et les **divergences**, plutôt que de désigner un gagnant.
- Servir autant celles et ceux qui **créent** du contenu (une minorité) que celles et ceux qui veulent **s'informer et réfléchir**.

Voir la vision complète dans [`vision/manifeste.md`](vision/manifeste.md).

## Comment ça marche (en bref)

Le dépôt est un cycle vivant. Chaque étape est un dossier, chaque contribution est un fichier Markdown versionné par Git (la mémoire du mouvement des idées) :

1. **Idées** → [`idees/`](idees/) : on dépose une graine (problème, intuition, proposition) **avec un slogan / expression associée**.
2. **Points de vue** → [`points-de-vue/`](points-de-vue/) : on confronte, avec l'obligation de défendre honnêtement (*steelman*) la position adverse.
3. **Synthèses** → [`syntheses/`](syntheses/) : l'IA cartographie convergences, divergences et angles morts, à plusieurs échelles.
4. **Slogans** → [`slogans/`](slogans/) : on distille les consensus en idées fortes, avec le raisonnement derrière.
5. **Décisions** → [`decisions/`](decisions/) : on consigne les choix structurants (format ADR léger).

Le processus complet est décrit dans [`workflow/processus.md`](workflow/processus.md) et les rôles (humains + IA) dans [`workflow/roles.md`](workflow/roles.md).

## Comment contribuer

- Toute contribution passe par une **Pull Request** (humaine ou proposée par l'IA), relue par au moins un humain.
- Copie le gabarit `_gabarit-*.md` du dossier concerné, remplis-le, ouvre une PR.
- Les règles de collaboration avec l'IA sont dans [`AGENTS.md`](AGENTS.md).

## Structure du dépôt

```
vision/        # Le pourquoi : manifeste, valeurs, glossaire commun
idees/         # Les graines d'idées
points-de-vue/ # Les débats structurés (thèse, pour, contre, nuances)
syntheses/     # Les cartes convergence/divergence produites avec l'IA
slogans/       # Les idées fortes distillées (+ noyau/ d'axiomes)
decisions/     # Le journal des décisions structurantes (ADR light)
archive/       # Hors circuit actif, sans effacer
workflow/      # Le processus et les rôles
AGENTS.md      # Les règles de collaboration avec l'IA
```

## Statut

Projet exploratoire, mené par y-magma et Vincent. Rien n'est figé : la forme de l'outil est elle-même une des questions ouvertes du dépôt.
