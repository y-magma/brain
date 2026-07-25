# 0001 — Conventions du Brain de Magma

- **Date** : 2026-07-25
- **Statut** : adoptée
- **Décideurs** : y-magma
- **Remplace** : anciennes 0001 (langue), 0002 (archive/vues), 0005 (chantiers)

## Contexte

Atelier Markdown pour inventer Magma. Pas de code applicatif ici. On peut **tout casser / refaire**.

## Décision

1. **Nom** : le projet s’appelle **Magma** ; ce dépôt est le **Brain** de Magma (repo GitHub `brain` OK).
2. **Langue** : français par défaut.
3. **Organisation** : uniquement des **chantiers** (`seed` / `debate` / `map` / `formula`). Pas de dossiers « étapes » legacy.
4. **Archive** : `archive/graines/` pour le hors-circuit, sans effacer.
5. **Pas de code** : pas d’app à build ; illustrations / CSS de lecture OK.
6. **Tout casser** : structure, ton, noyau — refonte autorisée via PR ; pas de sacralisation.
7. **PR humaine** : l’IA propose ; un humain fusionne.

## Conséquences

- Simplicité de navigation.
- Migration unique ; plus de stubs « legacy ».
- À revisiter si Magma produit sort du Markdown (autre repo).
