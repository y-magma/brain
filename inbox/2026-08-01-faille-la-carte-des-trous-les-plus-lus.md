# Proposition — Faille (la carte des trous les plus lus)

- **Date** : 2026-08-01
- **Par** : IA (demande Ariel)
- **Nature** : outil-magma *(proposition — nom provisoire)*
- **Attention** : brut
- **Tags** : wikipedia, qualité, attention, chantiers

## En une phrase

Croiser **ce qui est faible** (phrases sans source, sections contestées, articles ébauches) avec **ce qui est massivement lu** : la carte des endroits où une heure de travail collectif vaut le plus.

## La porte (une seule)

Pas « où contribuer ? » mais **« où le trou coûte le plus cher ? »**.

## Nouvelle définition de la qualité

La qualité cesse d’être une note par article et devient une **allocation d’attention**. Une ébauche lue trois fois par an n’est pas un problème. Une phrase sans source lue deux millions de fois par an en est un.

| Signal faiblesse | Signal attention | Croisement |
|------------------|------------------|------------|
| `citation needed`, sections contestées, neutralité disputée | Consultations par mois | **Trou cher** |
| Article ébauche | Trafic saisonnier (actualité, examens) | Trou urgent |
| Source morte ou dépréciée | Nombre de pages qui en dépendent | Trou structurel |

## Données mobilisables *(faits vérifiables)*

- Modèles de maintenance : la Wikipédia anglophone recense plus de **579 000 articles** contenant au moins une affirmation non sourcée ([Category:All articles with unsourced statements](https://en.wikipedia.org/wiki/Category:All_articles_with_unsourced_statements)).
- Modèles de qualité d’article via [Lift Wing](https://wikitech.wikimedia.org/wiki/Machine_Learning/LiftWing) — les anciens modèles ORES y sont servis mais **dépréciés** ; l’équipe recommande les modèles récents, multilingues. À traiter comme une estimation, pas un verdict.
- Consultations via l’API Pageviews ; jeux de données analytiques en **CC0**.

**Ce qui existe déjà** : [Citation Hunt](https://meta.wikimedia.org/wiki/Citation_Hunt) propose des extraits non sourcés au hasard ; [PetScan](https://en.wikipedia.org/wiki/Wikipedia:PetScan) croise des catégories.  
**Ce qui manquerait** *(hypothèse)* : la **priorisation par impact** — et surtout, transformer chaque trou en **question** posée à un collectif, puis suivre si elle a été refermée.

## Ce que ça ne fait pas

Ne modifie pas Wikipédia à la place des gens, ne juge pas les contributeurs, ne produit pas de contenu automatique, ne remplace pas les processus éditoriaux de la communauté.

## Garde-fous

- **Volume n’est pas qualité** : mesurer les trous refermés et tenus, jamais le nombre de modifications.
- Ne pas diriger une foule extérieure vers des pages sensibles — risque réel de brigading. Les sujets à forte tension sont signalés et sortis du flux public.
- Respect explicite des règles de la communauté ; l’outil forme avant d’envoyer.
- Le classement « trou cher » reste discutable et affiché comme tel : c’est une hypothèse d’allocation, pas une vérité.

## Deux questions cobayes

- **« Faut-il interdire les écrans avant six ans ? »** → montre où les affirmations les plus reprises tiennent sur du vide, et à quel volume de lecture. Un chantier collectif devient concret : trois phrases précises à sourcer.
- **« Le vote obligatoire améliore-t-il la démocratie ? »** → repère les articles pays par pays où les chiffres circulent sans source, alors qu’ils nourrissent le débat français.

## Cousins

[Citation Hunt](https://meta.wikimedia.org/wiki/Citation_Hunt) · [PetScan](https://en.wikipedia.org/wiki/Wikipedia:PetScan) · [Lift Wing](https://wikitech.wikimedia.org/wiki/Machine_Learning/LiftWing) · [paysage](../chantiers/paysage-outils-existants/analyse.md)

## Suite possible

- [ ] chantier · [x] outils/ *(si nom + porte validés)* · [x] questions → `cas/`  
Relié : [science-wiki](../chantiers/science-wiki/) · [simplicite](../chantiers/simplicite/) · [TRI (allocation d’attention)](../TRI.md)
