# 0001 — Conventions du Brain de Magma

- **Date** : 2026-07-25
- **Statut** : adoptée
- **Décideurs** : y-magma
- **Remplace** : anciennes 0001 (langue), 0002 (archive/vues), 0005 (chantiers)

## Contexte

Atelier Markdown pour inventer Magma. Pas de code applicatif ici. On peut **tout casser / refaire**.

## Décision

1. **Nom** : **Magma** = projet / famille d’outils ; ce dépôt = **Brain** (repo `brain` OK).
2. **Langue** : français par défaut.
3. **Brain** : organisation par **chantiers** (`seed` / `debate` / `map` / `formula`) — atelier, pas UX outil.
4. **Outils Magma** : catalogue [`../outils/`](../outils/) — chaque outil a un **nom** (ex. Weco) ; catalyse *une partie* des idées. On ne dit plus « instance ».
5. **Exemples de questions** : [`../chantiers/banc-essai-debats/cas/`](../chantiers/banc-essai-debats/cas/) — distincts des outils ; adaptables.
6. **Archive** : `archive/graines/`.
7. **Pas de code applicatif** ici.
8. **Tout casser** (Brain) via PR ; PR humaine obligatoire.

## Conséquences

- Trois couches lisibles : idées · outils · exemples.
- Risque de re-fusionner Weco dans les « cas » — résisté dans en-clair.
- À revisiter quand un 2ᵉ outil Magma apparaît.
