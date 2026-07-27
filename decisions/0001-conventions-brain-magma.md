# 0001 — Conventions du Brain de Magma

- **Date** : 2026-07-25
- **Statut** : adoptée
- **Décideurs** : y-magma
- **Remplace** : anciennes 0001 (langue), 0002 (archive/vues), 0005 (chantiers)

## Contexte

Atelier Markdown pour inventer Magma. Pas de code applicatif ici. On peut **tout casser / refaire**.

## Décision

1. **Nom** : le projet produit s’appelle **Magma** ; ce dépôt est le **Brain** (repo `brain` OK).
2. **Langue** : français par défaut.
3. **Organisation du Brain** : **chantiers** (`seed` / `debate` / `map` / `formula`). Convention d’*atelier*, pas spécification UX Magma.
4. **Magma ≠ Brain** : Magma vise le *pour tous* / structure plutôt **plate** ; le Brain peut rester exigeant et évolutif — **exemple** de brainstorming, pas le miroir du produit.
5. **Archive** : `archive/graines/` hors circuit, sans effacer.
6. **Pas de code applicatif** ici ; illustrations / CSS de lecture OK.
7. **Tout casser** (côté Brain) : via PR ; pas de sacralisation.
8. **PR humaine** : l’IA propose ; un humain fusionne.

## Conséquences

- Clarté atelier.
- Risque de confusion Magma/Brain — à rappeler dans [`../workflow/en-clair.md`](../workflow/en-clair.md).
- À revisiter si Magma produit sort dans un autre repo (probable).
