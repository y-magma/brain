# Voir `brain` simplement, comme un humain

Le dépôt est du Markdown : c'est volontaire (lisible par les humains **et** par l'IA, versionné par Git). Voici trois façons de le « voir », du zéro-effort au plus confortable.

## Niveau 0 — GitHub (rien à installer)

- Le fichier [`../CARTE.md`](../CARTE.md) est la **page d'accueil humaine** : l'état de la pensée en un coup d'œil.
- GitHub affiche déjà tout le Markdown proprement, et les `README.md` de chaque dossier servent d'index.
- L'onglet « History » et les Pull Requests montrent le **mouvement des idées**.

C'est suffisant pour commencer à deux avec Vincent.

## Niveau 1 — Un vrai « site wiki » sans build : Docsify

[Docsify](https://docsify.js.org) transforme le dossier en site (barre latérale, recherche) **sans étape de compilation** : un seul fichier `index.html` lit les `.md` à la volée.

Pour le voir en local :

```bash
# depuis la racine du dépôt
python3 -m http.server 8000
# puis ouvrir http://localhost:8000 dans le navigateur
```

La barre latérale est définie dans [`../_sidebar.md`](../_sidebar.md). Pour publier en ligne : activer **GitHub Pages** sur la branche, le site se sert tout seul (toujours zéro build).

## Niveau 2 — Vue « cerveau » : Obsidian

Ouvrir le dossier comme *vault* dans [Obsidian](https://obsidian.md) (gratuit) donne :

- une **vue graphe** des liens entre idées, débats et synthèses ;
- l'édition Markdown confortable, la recherche, les backlinks.

Idéal pour naviguer la pensée comme un réseau plutôt qu'une arborescence.

---

### Quel niveau choisir ?

| Besoin | Niveau |
|--------|--------|
| Jeter un œil, contribuer à deux | 0 (GitHub + `CARTE.md`) |
| Partager un site lisible au public | 1 (Docsify + GitHub Pages) |
| Explorer les liens entre idées | 2 (Obsidian) |

> Rappel : ces vues ne changent rien au fond. La règle reste « un fichier = une contribution, relue en Pull Request ».
