# En clair — à quoi sert le Brain, et quoi faire d’une idée

> Lis **ça** si le reste te perd. Une page. Point.

## Deux noms, un atelier

| Nom | C’est quoi |
|-----|------------|
| **Magma** | Le *projet* : inventer une machine à penser / un outil de démocratie (forme encore ouverte). |
| **Brain** | *Ce dépôt GitHub* : l’atelier où Ariel, Vincent (+ l’IA) pensent Magma **avant** (et pendant) le produit. |

Le Brain **n’est pas** (encore) l’app grand public.  
Il **aide** à : poser des questions, confronter sans se mentir, cartographier, distiller des formules, trancher peu — et **garder la mémoire**.

Sans Brain : idées dans des chats qui disparaissent.  
Avec Brain : une idée a un *lieu*, un *historique*, une *suite*.

### Banc d’essai (débats cobayes)

Pour tester ce que Magma **jugera** un jour :  
→ [`../chantiers/banc-essai-debats/`](../chantiers/banc-essai-debats/)  
Exemple : [`../chantiers/banc-essai-debats/cas/supprimer-le-patrimoine/`](../chantiers/banc-essai-debats/cas/supprimer-le-patrimoine/) — « Faut-il supprimer le patrimoine ? »

---

## Workflow d’une idée (le seul qu’il faut retenir)

```
1. SEED      →  tu poses l’idée + un slogan
2. DEBATE    →  tu écoutes le pour ET le contre (steelman)
3. MAP       →  tu notes accords / désaccords / trous
4. FORMULA   →  tu gardes la phrase qui reste vraie
5. (parfois) DÉCISION ou ARCHIVE
```

**Un sujet = un dossier** dans `chantiers/<sujet>/` :

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
- **Ne fait pas** : décider à ta place, fusionner les PR, imposer un dogme.

---

## Comment le Brain « aide » Magma (sans blabla)

1. **Frein anti-bazar** — une idée n’explose pas en 12 fichiers orphelins.  
2. **Frein anti-ego** — steelman obligatoire : tu défends l’autre camp.  
3. **Frein anti-dogme** — tout est rouuvrable ([questions sans dogme](../chantiers/questions-sans-dogme/)).  
4. **Accélérateur de clarté** — slogan d’abord ; profondeur par liens.  
5. **Mémoire** — Git = on voit le mouvement des idées.  
6. **Pont vers l’art** — la fiction absurde peut *activer* autrement que le débat front ([fiction absurde](../chantiers/fiction-absurde/)).  
7. **Banc d’essai** — débats cobayes pour prototyper le jugement Magma ([banc d’essai](../chantiers/banc-essai-debats/)).

---

## Ce que le Brain n’est pas

- Pas un réseau social.  
- Pas « on a révolutionné la démocratie » (voir [une porte, pas tout](../chantiers/une-porte-pas-tout/)).  
- Pas du code produit — c’est de la **pensée versionnée**.

Détail ton : [`ton.md`](ton.md) · Rôles : [`roles.md`](roles.md) · Carte : [`../CARTE.md`](../CARTE.md)
