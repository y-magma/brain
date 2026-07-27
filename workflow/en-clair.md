# En clair — à quoi sert le Brain, et quoi faire d’une idée

> Lis **ça** si le reste te perd. Une page. Point.

## Deux noms — ne pas les confondre

| Nom | C’est quoi | Forme |
|-----|------------|--------|
| **Magma** | L’outil *pour tous* qu’on invente (démocratie / machine à penser). | Plutôt **plate** : entrer vite, peu de dossiers à apprendre. Forme encore ouverte. |
| **Brain** | *Ce* dépôt : atelier Ariel + Vincent (+ IA) pour **brainstormer Magma**. | Se **structure progressivement** (chantiers…) — **exemple** de brainstorming versionné, **pas** le modèle UI de Magma. |

**Attention :** la profondeur du Brain (seed / debate / map / formula, nombreux chantiers) sert à *penser le produit*.  
Ce n’est **pas** le brief « Magma = un GitHub avec 12 dossiers ». Magma doit rester accessible ; le Brain peut rester exigeant.

Le Brain **aide** à : poser des questions, confronter sans se mentir, cartographier, distiller, trancher peu, garder la mémoire — et **montrer** une façon de brainstormer.

Sans Brain : idées dans des chats qui disparaissent.  
Avec Brain : une idée a un *lieu*, un *historique*, une *suite* (pour l’équipe).

### Banc d’essai (débats cobayes)

Matériaux pour prototyper ce que Magma pourra accueillir / juger — **pas** la structure de l’app.  
→ [`../chantiers/banc-essai-debats/`](../chantiers/banc-essai-debats/)  
Ex. [patrimoine](../chantiers/banc-essai-debats/cas/supprimer-le-patrimoine/) · [Weco](../chantiers/banc-essai-debats/cas/weco/) ([Pages `/weco/`](https://y-magma.github.io/weco/)).

---

## Workflow d’une idée **dans le Brain** (atelier)

```
1. SEED      →  tu poses l’idée + un slogan
2. DEBATE    →  tu écoutes le pour ET le contre (steelman)
3. MAP       →  tu notes accords / désaccords / trous
4. FORMULA   →  tu gardes la phrase qui reste vraie
5. (parfois) DÉCISION ou ARCHIVE
```

**Un sujet = un dossier** `chantiers/<sujet>/` *(convention Brain, pas spec Magma)* :

| Fichier | Question qu’il répond |
|---------|------------------------|
| `seed.md` | De quoi on parle, et en une phrase ? |
| `debate.md` | Quel est le meilleur argument de chaque camp ? |
| `map.md` | Sur quoi on s’accorde / on diverge / on est aveugle ? |
| `formula.md` | Quelle formule on peut répéter sans mentir ? |

Tu n’es **pas** obligé de tout remplir le jour 1.  
Mais : **pas de `map.md` = boucle ouverte** (on le voit exprès).

### Exemple ultra concret

Idée : « et si on faisait un atlas de slogans ? »

1. Créer `chantiers/atlas-slogans/seed.md` + slogan  
2. Dans `debate.md` : atlas curaté vs réseau social (déjà fait)  
3. Dans `map.md` : encore à écrire ← le prochain pas utile  
4. Dans `formula.md` : « ralentir les slogans sans les tuer »

Quand c’est mûr → éventuellement une **décision** dans `decisions/`.  
Quand c’est en pause → `archive/graines/`.

### Ce que l’IA fait / ne fait pas

- **Fait** : reformuler, steelman, cartographier, proposer des formules, relier.  
- **Ne fait pas** : décider à ta place, fusionner les PR, imposer un dogme, **décider la UX Magma à ta place**.

---

## Comment le Brain « aide » Magma (sans blabla)

1. **Laboratoire d’idées** — beaucoup de pistes ; on trie sans tout livrer.  
2. **Exemple de brainstorming** — méthode vivante, pas statue.  
3. **Frein anti-ego** — steelman.  
4. **Frein anti-dogme** — tout rouuvrable.  
5. **Mémoire** — Git.  
6. **Ne pas coller** la complexité atelier → produit grand public.  
7. Pont art / banc d’essai / sœurs (Weco) = **matériaux**, pas l’architecture Magma.

---

## Ce que le Brain n’est pas

- Pas Magma-pour-tous (l’app).  
- Pas un réseau social.  
- Pas « on a révolutionné la démocratie » (voir [une porte, pas tout](../chantiers/une-porte-pas-tout/)).  
- Pas du code produit — **pensée versionnée** + exemple de méthode.

Détail ton : [`ton.md`](ton.md) · Rôles : [`roles.md`](roles.md) · Carte : [`../CARTE.md`](../CARTE.md)
