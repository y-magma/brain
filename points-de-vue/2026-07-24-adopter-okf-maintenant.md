# Débat : faut-il adopter OKF maintenant pour `brain` / l'outil grand public ?

- **Date** : 2026-07-24
- **Animé par** : IA (steelman des deux camps, à partir d'une question de y-magma)
- **Idée(s) source** : [`../idees/2026-07-24-open-knowledge-format-et-brain.md`](../idees/2026-07-24-open-knowledge-format-et-brain.md), [`../idees/2026-07-23-un-outil-de-democratie.md`](../idees/2026-07-23-un-outil-de-democratie.md)
- **Statut** : ouvert

## La thèse en débat

Pour construire des outils grand public et pour faire avancer la recherche collaborative à deux sur une « machine à penser », **nous devrions utiliser dès maintenant le Open Knowledge Format (OKF)** comme format de connaissance du dépôt `brain` (et comme cible d'échange du futur produit).

## Arguments POUR (steelman)

1. **Vous êtes déjà sur le motif qu'OKF formalise.** Markdown + Git + agents qui lisent le même corpus : c'est exactement le « LLM-wiki » que Google Cloud dit standardiser. Adopter tôt, c'est éviter de réinventer des conventions (frontmatter, `type`, chemins comme identité) que d'autres agents comprendront demain sans adaptateur.
2. **Coût d'adoption minimal.** OKF v0.1 n'exige qu'un champ `type` ; le reste reste libre. On peut garder le cycle idées → débats → synthèses, et seulement ajouter un frontmatter YAML. Ce n'est pas migrer vers une plateforme Google.
3. **Portabilité = souveraineté.** Si le but est un outil de démocratie non capturé, un format d'échange ouvert (lisible hors compte cloud, hors SDK) est un atout : d'autres outils, d'autres IA, d'autres collectifs peuvent consommer la même connaissance.
4. **Anticipe le produit grand public.** Même si aujourd'hui on est deux, le jour où l'outil exporte « une idée multi-points-de-vue » vers d'autres systèmes, avoir déjà un bundle OKF évite une réécriture douloureuse.
5. **Les agents aiment le peu de structure.** Distinguer `type: idee` / `type: debat` / `type: synthese` (et tags, timestamps) rend le dépôt filtrable et navigable pour l'IA sans sacrifier la prose humaine — aligné avec le rôle de l'IA dans [`../AGENTS.md`](../AGENTS.md).

## Arguments CONTRE (steelman)

1. **Mauvais problème, mauvais moment.** La question ouverte du manifeste n'est pas « quel format de fichiers ? », c'est « quelle *forme* pour l'outil de démocratie ? ». OKF ne répond pas au multi-échelle, au steelman obligatoire, ni au spectacle du désaccord. Optimiser l'infra avant le modèle mental, c'est de la procrastination élégante.
2. **OKF n'est pas fait pour ce contenu.** Les exemples officiels parlent de tables BigQuery, métriques, runbooks, catalogues de données. `brain` travaille des *positions*, *divergences de valeurs*, *slogans traçables*. Rien n'interdit d'étendre OKF, mais le standard n'apporte pas encore de vocabulaire pour ça — on inventerait un dialecte « brain-OKF » de toute façon.
3. **Effet d'autorité / faux dilemme.** « Google a publié un format ouvert » ≠ « nous devons l'utiliser ». Le sophisme guette : traiter un vendeur cloud comme arbitre de la bonne manière de penser. Un format maison clair + export ultérieur peut suffire.
4. **Friction pour deux humains.** YAML, conformité, types : coût cognitif et de relecture pour un atelier exploratoire. Le gabarit Markdown actuel est déjà la contrainte minimale qui marche. Toute convention supplémentaire doit prouver sa valeur *maintenant*.
5. **Standard trop jeune.** v0.1, écosystème naissant, trajectoire incertaine hors Google Cloud Knowledge Catalog. Parier tôt peut verrouiller sur une cible qui bouge ou qui reste niche.

## Positions absentes / minoritaires

- **« Ni adoption, ni ignorance : couche d'export. »** Garder le format éditorial `brain` tel quel ; le jour où un produit a besoin d'interopérabilité, écrire un producteur OKF (comme Google fournit des producteurs pour BigQuery). Le format interne ≠ le format d'échange.
- **« OKF pour le *produit*, pas pour l'*atelier*. »** L'atelier reste libre et humain-first ; le runtime grand public (si agents, si partage entre apps) parle OKF.
- **« S'inspirer sans se conformer. »** Reprendre les principes OKF (un concept = un fichier, liens Markdown, peu de champs queryables) sans viser la conformité ni le branding Google.
- **« Schema.org / vocabulaire du débat public. »** Si l'outil vise le web grand public, le problème de découverte (schema.org, pages web) est distinct de celui d'OKF (agents / catalogues internes). Les deux peuvent coexister plus tard.

## Présupposés cachés

- Que « machine à penser » implique nécessairement une base de connaissance *consommée par des agents tiers* (sinon OKF est moins pertinent).
- Que l'interopérabilité vaut plus, à ce stade, que la vitesse d'exploration conceptuelle à deux.
- Que se rapprocher d'un format Google Cloud n'introduit pas, même symboliquement, une dépendance narrative (« on construit sur leur stack ») — tension possible avec l'outil de démocratie indépendant.
- Que le Markdown actuel de `brain` est « assez » pour les agents (AGENTS.md + gabarits) sans frontmatter.

## Nuances et cas particuliers

| Situation | Lecture plausible |
|-----------|-------------------|
| Atelier à 2, recherche de forme | OKF **non bloquant** ; veille utile, adoption lourde prématurée |
| Export vers d'autres agents / outils | OKF (ou équivalent) devient **pertinent** comme format d'échange |
| Catalogue de faits / sources / métriques dans le produit | Cas d'usage **proche** des exemples OKF |
| Représentation multi-points-de-vue, divergences de valeurs | Cas d'usage **loin** du cœur OKF actuel → modèle maison d'abord |
| SEO / découverte web grand public | Problème **différent** (schema.org, etc.), ne pas confondre |

## Ce qui surprend / fait bouger l'avis

Le faux dilemme se dissout : **ce n'est pas « OKF ou pas OKF pour tout le projet ».**  
`brain` peut rester un atelier de pensée en Markdown libre *et* OKF peut être pertinent plus tard comme **protocole d'échange** pour un outil grand public — sans que l'un décide de l'autre aujourd'hui.

Ce qui déplace vraiment le débat : clarifier si la « machine à penser » doit **être** un corpus d'agents portables, ou **produire** des expériences de débat pour des humains (avec éventuellement un export machine en sous-produit).

## Questions ouvertes

1. Dans 6–12 mois, le produit doit-il exposer un bundle lisible par n'importe quel agent tiers ?
2. Quels *types* de documents `brain` voudrait-il standardiser (`idee`, `debat`, `synthese`, `slogan`, `decision`) — et cela mérite-t-il un vocabulaire publié ?
3. Un frontmatter minimal (`type`, `statut`, `echelles`) sans revendiquer OKF serait-il un bon compromis immédiat ?
4. Qui décide, et sur quel critère (interopérabilité mesurable vs friction de rédaction) ?

## Vers la synthèse

Quand y-magma et Vincent auront tranché (ou assumé une divergence) sur « atelier vs produit » et « format interne vs format d'échange », ouvrir une carte dans [`../syntheses/`](../syntheses/) — puis, si besoin, un ADR dans [`../decisions/`](../decisions/).
