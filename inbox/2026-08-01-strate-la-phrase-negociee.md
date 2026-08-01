# Proposition — Strate (la phrase négociée)

- **Date** : 2026-08-01
- **Par** : IA (demande Ariel)
- **Nature** : outil-magma *(proposition — nom provisoire)*
- **Attention** : brut
- **Tags** : wikipedia, qualité, steelman, mémoire

## En une phrase

Chaque phrase de Wikipédia est le **dépôt d’une négociation** ; Strate la rouvre : combien de fois elle a été contestée, par quel argument, ce qui a été retiré, et pourquoi la version actuelle a tenu.

## La porte (une seule)

Pas « est-ce vrai ? » mais **« combien a coûté cet accord ? »**.

## Nouvelle définition de la qualité

Aujourd’hui la qualité se lit comme un **état** (un label, une étoile).  
Ici elle se lit comme une **épreuve traversée** : une phrase qui a survécu à quinze contestations argumentées n’a pas le même statut qu’une phrase que personne n’a jamais lue.

| Signal | Ce qu’il dit |
|--------|--------------|
| Nombre de révocations sur ce passage | Zone disputée ou zone morte |
| Arguments de la page de discussion liés à ce passage | La raison, pas juste l’auteur |
| Texte supprimé et jamais réinséré | Ce que le consensus a refusé |
| Âge du passage + trafic de la page | Consensus éprouvé ou angle mort |

## Données mobilisables *(faits vérifiables)*

- Historique complet des révisions et pages de discussion, via l’[API MediaWiki](https://www.mediawiki.org/wiki/API:Main_page) et les [dumps](https://dumps.wikimedia.org/).
- Attribution au niveau du mot via [WikiWho / WhoColor](https://www.mediawiki.org/wiki/WikiWho/en), qui alimente déjà l’extension [Who Wrote That?](https://www.mediawiki.org/wiki/Who_Wrote_That).
- Licence : texte en **CC BY-SA 4.0** depuis juin 2023 — attribution et partage à l’identique obligatoires.

**Ce qui manque aujourd’hui** *(hypothèse, à vérifier)* : les outils existants disent **qui** a écrit, pas **quel argument** a fait tenir la phrase. Le chaînon passage ↔ discussion ↔ verdict n’est pas outillé pour un lecteur ordinaire.

## Ce que ça ne fait pas

Ne note pas les contributeurs, ne rejuge pas les guerres d’édition, ne dit pas quel camp avait raison, ne remplace pas l’historique officiel.

## Garde-fous

- **Ancienneté n’est pas vérité** : une phrase peut survivre par inattention. Le signal « jamais discutée » est affiché comme tel, pas comme un gage.
- Aucun profil d’éditeur, aucun classement de personnes.
- Attribution CC BY-SA respectée sur chaque extrait affiché.

## Deux questions cobayes

- **« Faut-il supprimer le patrimoine ? »** → sur les articles de restitution d’œuvres, Strate montre quelles phrases ont été réécrites vingt fois et quel argument a tranché. Le [cas existant](../chantiers/banc-essai-debats/cas/supprimer-le-patrimoine/) gagne un matériau réel plutôt qu’imaginé.
- **« Le nucléaire est-il écologique ? »** → la page bouge à chaque rapport ; Strate rend visible ce qui est stabilisé (physique, coûts constatés) et ce qui se rejoue à chaque actualité.

## Cousins

[Who Wrote That?](https://www.mediawiki.org/wiki/Who_Wrote_That) · [XTools](https://www.mediawiki.org/wiki/XTools) · analyse du [paysage](../chantiers/paysage-outils-existants/analyse.md)

## Suite possible

- [ ] chantier · [x] outils/ *(si nom + porte validés)* · [x] questions → `cas/`  
Relié : [science-wiki](../chantiers/science-wiki/) · [atlas-slogans](../chantiers/atlas-slogans/) · [histoires partagées](../chantiers/histoires-fictions-partagees/)
