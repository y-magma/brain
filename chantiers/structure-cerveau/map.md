# Map — critique de la structure de `brain`

> Migrée ici depuis `syntheses/` (chantier = lieu unique). Ton : on garde le fond, on assume le tranchant.


- **Date** : 2026-07-25
- **Rédigée par** : IA — **Relue par** : _(en attente)_
- **Débat(s) source** : observation du dépôt (états des dossiers) ; [`../../workflow/processus.md`](../../workflow/processus.md) ; [`../../decisions/0001-langue-et-methode-de-travail.md`](../../decisions/0001-langue-et-methode-de-travail.md) ; [`../../decisions/0002-archivage-vues-et-noyau-slogans.md`](../../decisions/0002-archivage-vues-et-noyau-slogans.md) ; graine [`seed.md`](seed.md) · décision [`../../decisions/0005-structure-par-chantiers.md`](../../decisions/0005-structure-par-chantiers.md)

## En une phrase

Le cycle en 5 étapes est une **bonne hygiène de pensée**, mais trop lourd pour 2 humains + IA : on produit surtout des graines, on ferme peu de boucles — et le dépôt mélange *atelier pour inventer l'outil* et *prototype de l'outil*.

## Steelman de la structure actuelle

Avant critique : la structure défend quelque chose de fort.

1. **Pipeline = discipline anti-populisme.** Idée → confrontation (steelman) → carte → formule → décision empêche le slogan orphelin et le « on a tranché » sans carte.
2. **Git + PR = mémoire et frein.** Versionner le mouvement des idées ; l'humain garde le veto (aligné manifeste).
3. **Séparation des natures de documents** aide l'IA et les humains à savoir *quel type de travail* faire (explorer ≠ cartographier ≠ décider).
4. **Archive + Carte + noyau** (0002) répondent déjà au bruit : ne pas effacer, voir par étape, boussole minimale.

Ce n'est pas une structure « naïve ». C'est une structure **exigeante** — et c'est là que le coût apparaît.

## Faits observables (dépôt, 2026-07-25)

| Zone | Fichiers de contenu (hors README/gabarits) |
|------|-------------------------------------------|
| `idees/` actives | 9 |
| `points-de-vue/` | 3 |
| `syntheses/` | **0** (avant cette carte) |
| `slogans/` (hors noyau) | 0 · noyau candidats : 1 |
| `decisions/` | 4 (2 adoptées, 2 proposées) |
| `archive/` | **11** idées + 1 débat |

**Lecture** : beaucoup d'entrée (`idees` + archive), peu de sortie (`syntheses` / slogans distillés). Le livrable principal annoncé pour l'IA (synthèses) était le trou structurel.

## Convergences (ce sur quoi on peut s'accorder sans trancher le fond)

- On cherche une **machine à penser / outil de démocratie**, forme encore ouverte.
- **Peu de verbalisation** + phrases courtes = brique majeure (0003/0004 proposées).
- L'IA **cartographie**, les humains **décident**.
- Git comme mémoire reste un atout (pas un bug).
- Besoin d'une **vue humaine d'un coup d'œil** (Carte) — déjà reconnu.

## Divergences assumées

| Désaccord | Nature | Ce qui le sous-tend |
|-----------|--------|---------------------|
| Pipeline strict (5 dossiers) vs page vivante par *chantier* | valeur / hypothèse | Rigueur anti-populisme vs vitesse de boucle pour petit collectif |
| Le dépôt *est* le produit vs le dépôt *invente* le produit | valeur | Prototype méthodologique vs atelier de design |
| PR pour chaque graine vs inbox légère puis PR aux jalons | hypothèse | Qualité vs friction cognitive |
| Slogan = 4 usages (accroche / distillé / axiome / objet d'enquête) | fait + coût | Richesse sémantique vs confusion opérationnelle |

## Angles morts

- **Pas d'objet « chantier / fil »** : un sujet (ex. atlas) est éclaté en 3–4 idées + 1 débat sans dossier commun.
- **Pas de critère de « boucle fermée »** : quand une graine a « assez » vécu pour exiger synthèse ou archive.
- **Littérature / projets cousins peu reliés** au dépôt (voir ci-dessous) — on réinvente sans ancrage.
- **Coût de maintenance** (Carte + sidebar + README d'index + archive miroir) non budgété comme dette.
- **Échelle 2 personnes** : structure conçue comme si le collectif était déjà large.

## Où tu veux en venir (lecture cartographe)

Hypothèse de lecture (à corriger par les humains) :

1. **Inventer la forme** d'un outil qui rend le désaccord fécond et les formules traçables.
2. **Travailler déjà comme** on voudrait que l'outil fasse travailler — d'où le wiki-LLM.
3. **Ne pas se faire manger** par Twitter/populisme ni par encyclopédie morte.
4. Tension : *(2)* pousse à formaliser tôt ; *(1)* exige de rester léger pour explorer.

La structure actuelle privilégie *(2)* au détriment de *(1)* : on a un **processus de revue** plus qu'un **cerveau navigable**.

## Familles d'outils proches (littérature & projets)

| Famille | Exemples | Ce qu'ils font bien | Ce que `brain` a en plus / en moins |
|---------|----------|---------------------|-------------------------------------|
| **IBIS** (Issue / Position / Argument) | Kunz & Rittel ; MIT Deliberatorium ; DebateGraph | Graphe typé, pas pipeline linéaire | `brain` a steelman + slogans + Git ; pas de nœuds typés |
| **Argument mapping** | Kialo, Argdown, Rationale | Pour/contre arborescent, pédagogique | Moins de distillation / axiomes ; UI dédiée |
| **Opinion clustering** | [Pol.is](https://pol.is) | Consensus & fractures *sans* fil toxique | Pas d'encyclopédie permanente ; scale crowds |
| **Démocratie participative** | Loomio, Decidim, Consul | Propositions + votes + gouvernance | Moins « pensée » / slogans ; plus « décision publique » |
| **Wiki-LLM / second brain** | Karpathy LLM wiki, [yopedia](https://github.com/yologdev/yopedia), vaults Obsidian | Page vivante, anti-RAG, agents | Souvent 1 cerveau perso ou agents ; peu de steelman démocratique |
| **Consensus multi-agents Markdown** | [llm-wiki-coordination](https://github.com/AEVYRA/llm-wiki-coordination), turnfile | Protocoles d'accord agent + audit | Plus outillé, moins « démocratie humaine » |

**Fait** : tu n'es pas seul sur ce terrain.  
**Hypothèse** : l'originalité de `brain` serait l'intersection *phrases courtes traçables × steelman × cartographie × petit collectif humain+IA* — pas le pipeline à 5 dossiers.

## Alternatives (carte, pas verdict)

### A. Garder le pipeline, alléger (réforme minimale)

- Forcer **1 synthèse / semaine** ou dès qu'un débat a 2 steelmans.
- **Inbox** : graines en issue GitHub ou `inbox/` sans PR ; PR seulement débat / synthèse / décision.
- Fusionner mentalement **idée + point de vue** tant que le sujet est jeune (un seul fichier « en tension »).
- Un seul point d'entrée humain : **Carte** ; README = porte courte.

### B. Structure par *chantiers* (recommandation candidate)

Un dossier `chantiers/<slug>/` avec pages vivantes :

```
seed.md      # graine + slogan
debate.md    # steelman pour/contre (évolutif)
map.md       # convergences / divergences / angles morts
formula.md   # formule(s) candidates + raisonnement
```

Statut du chantier dans un front-matter. `decisions/` reste transversal. Archive = déplacer le dossier entier.

→ Détail : [`seed.md`](seed.md) · **adopté** via [`../../decisions/0005-structure-par-chantiers.md`](../../decisions/0005-structure-par-chantiers.md).

### C. Wiki plat type Wikipédia / LLM-wiki

Peu de dossiers ; **une page par concept** ; historique Git = versions. Labels (graine / carte / axiome) dans le YAML. Proche de l'intuition « Wikipédia 2.0 » du manifeste.

### D. Graphe IBIS (fichiers = nœuds)

`issues/`, `positions/`, `arguments/` (ou tags) + liens. Visualisation plus tard (Obsidian, Argdown). Fort pour la démocratie argumentée ; plus loin de « slogan d'abord ».

### E. Pol.is-first puis atlas

Sessions de clustering d'opinions → phrases de consensus/fracture → fiches. Inverse le pipeline actuel (d'abord le public, ensuite l'encyclopédie).

## Lecture multi-échelle

- **Individu (contributeur)** : trop de gabarits / dossiers = friction ; risque d'abandonner avant la synthèse.
- **Communauté (y-magma + Vincent)** : archive > actives = signal que le filtre d'entrée est trop bas ou la clôture trop haute.
- **Société (si ouverture)** : pipeline 5 étapes + GitHub PR = barrière forte pour non-dev ; ok pour atelier fondateur, mauvais pour « outil de démocratie » grand public.
- **Humanité** : ambition manifeste intacte ; structure actuelle = **échafaudage de chantier**, pas encore la forme du commun.

## Incertitudes et sources

- Incertain : si B (chantiers) suffit ou s'il faut C/D pour le produit final.
- Incertain : part de la dette due à la jeunesse (3 jours de dépôt) vs défaut de design.
- Sources : Pol.is (Small et al. / CompDem) ; Deliberatorium (Klein, MIT) ; Kialo (argument mapping éducatif) ; IBIS (Kunz & Rittel) ; projets wiki-LLM cités ci-dessus. Pas d'évaluation empirique *in situ* de `brain` au-delà des comptes de fichiers.

## Suites possibles

1. Débattre / trancher **A vs B** (réforme légère vs chantiers) — brouillon ADR si les humains le demandent.
2. Remplir les synthèses manquantes *produit* : atlas vs réseau ; noyau vs catalogue (le trou n'était pas que méta).
3. Relier explicitement le glossaire aux familles d'outils (éviter réinvention isolée).
4. Slogan candidat de cette carte : **« Fermer des boucles, pas ouvrir des dossiers. »**
