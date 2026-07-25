# Voir le Brain de Magma simplement

Le dépôt est du Markdown : c'est volontaire (lisible par les humains **et** par l'IA, versionné par Git). Voici trois façons de le « voir », du zéro-effort au plus confortable.

## Niveau 0 — GitHub (rien à installer)

- Le fichier [`../CARTE.md`](../CARTE.md) est la **page d'accueil humaine** : l'état de la pensée en un coup d'œil.
- GitHub affiche déjà tout le Markdown proprement, et les `README.md` de chaque dossier servent d'index.
- L'onglet « History » et les Pull Requests montrent le **mouvement des idées**.

C'est suffisant pour commencer à deux avec Vincent.

## Niveau 1 — Un vrai « site wiki » sans build : Docsify

### « Sans build », ça veut dire quoi ?

La plupart des générateurs de site (Hugo, Jekyll, MkDocs, Docusaurus) demandent une étape de **compilation** : une commande transforme les `.md` en `.html` avant publication. **Docsify évite ça** : le navigateur lit les fichiers `.md` *à la volée* et les affiche. Donc pas d'installation, pas de commande de build, pas de dossier `dist/` à régénérer à chaque changement. Tu édites un `.md`, tu rafraîchis la page, c'est à jour.

### C'est quoi Docsify, concrètement ?

[Docsify](https://docsify.js.org) est une petite **librairie JavaScript** (un script). Notre `index.html` charge ce script, qui lit `CARTE.md`, `_sidebar.md` et les autres pages, et fabrique le site (barre latérale, recherche) directement dans le navigateur.

### Le CDN : qu'est-ce qui vient d'internet ?

Notre `index.html` récupère le script Docsify depuis un **CDN** (jsDelivr) — c'est-à-dire un serveur public qui héberge la librairie. Concrètement :

- **Le contenu** (tes `.md`) est servi depuis là où tu héberges le site (ta machine, ou GitHub Pages).
- **La librairie Docsify** (~quelques dizaines de Ko) est téléchargée depuis le CDN au chargement de la page.

Le lecteur a donc besoin d'un accès internet pour charger la librairie. Si tu veux **zéro dépendance externe**, on peut « embarquer » Docsify dans le dépôt (copier le `.js`/`.css` en local) — dis-le-moi et je le fais.

### Le voir en local

```bash
# depuis la racine du dépôt
python3 -m http.server 8000
# puis ouvrir http://localhost:8000 dans le navigateur
```

`http://localhost:8000` n'est visible que sur **ta** machine (utile pour tester).

### Obtenir une URL publique facilement (GitHub Pages)

Le plus simple, gratuit et lié au dépôt. Une fois cette branche fusionnée dans `main` :

1. Sur GitHub : **Settings → Pages**.
2. **Source** : « Deploy from a branch », branche `main`, dossier `/ (root)`.
3. Enregistrer. Après une minute, l'URL apparaît :
   **`https://y-magma.github.io/brain/`**

Aucune compilation : GitHub sert juste les fichiers, Docsify fait le rendu côté navigateur. Le fichier `.nojekyll` (à la racine) est indispensable pour que `_sidebar.md` soit bien servi.

> **Sidebar :** les liens de [`_sidebar.md`](../_sidebar.md) doivent rester en **chemins absolus** (préfixe `/`, ex. `/chantiers/README.md`). Le site active `relativePath` pour que les liens `../` *dans* les pages marchent ; sans `/` en tête, la sidebar résoudrait depuis la page courante et produirait des 404.

> Alternatives tout aussi simples pour une URL : déposer le dossier sur [Netlify Drop](https://app.netlify.com/drop) (glisser-déposer), ou `npx serve` en local.

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
