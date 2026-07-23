# Le processus

Un cycle vivant en cinq temps. Il n'est pas strictement linéaire : on peut boucler, revenir en arrière, rouvrir un débat clos. Git garde la trace du mouvement.

```
   ┌─────────┐   ┌───────────────┐   ┌────────────┐   ┌──────────┐   ┌────────────┐
   │  IDÉES  │──▶│ POINTS DE VUE │──▶│ SYNTHÈSES  │──▶│ SLOGANS  │──▶│ DÉCISIONS  │
   │ (graine)│   │  (confronter) │   │(cartograph.)│   │(distiller)│  │ (trancher) │
   └─────────┘   └───────────────┘   └────────────┘   └──────────┘   └────────────┘
        ▲                                    │                              │
        └────────────── rouvrir / itérer ◀───┴──────────────────────────────┘
```

## 1. Capturer une idée — `idees/`

N'importe qui (ou l'IA) dépose une **graine** : un problème, une intuition, une proposition.
- Copier [`../idees/_gabarit-idee.md`](../idees/_gabarit-idee.md).
- Nommer le fichier `AAAA-MM-JJ-titre-court.md`.
- Rôle de l'IA : reformuler, repérer les doublons, poser les bonnes questions.

## 2. Confronter — `points-de-vue/`

Pour une idée qui mérite débat, on ouvre un **point de vue structuré**.
- Copier [`../points-de-vue/_gabarit-debat.md`](../points-de-vue/_gabarit-debat.md).
- Remplir : thèse, meilleurs arguments **pour** (steelman), meilleurs arguments **contre** (steelman), nuances, présupposés, questions ouvertes.
- Rôle de l'IA : produire le *steelman* des positions absentes, révéler les présupposés cachés, signaler les sophismes.

## 3. Cartographier — `syntheses/`

Quand un débat a mûri, on en fait une **carte**.
- Copier [`../syntheses/_gabarit-synthese.md`](../syntheses/_gabarit-synthese.md).
- Distinguer : **convergences** (accords), **divergences assumées** (désaccords de valeurs), **angles morts**.
- Analyser aux échelles individu / communauté / société / humanité.
- Rôle de l'IA : c'est son livrable principal ; l'humain relit et corrige.

## 4. Distiller — `slogans/`

Un consensus solide se condense en une **idée forte et mémorable**.
- Copier [`../slogans/_gabarit-slogan.md`](../slogans/_gabarit-slogan.md).
- Toujours relier le slogan à son raisonnement et aux points de vue qu'il réconcilie. Pas de formule choc orpheline.
- Rôle de l'IA : proposer plusieurs formulations candidates ; l'humain choisit.

## 5. Trancher — `decisions/`

Les choix structurants (forme de l'outil, orientations) sont consignés.
- Copier [`../decisions/_gabarit-decision.md`](../decisions/_gabarit-decision.md) (format ADR léger : contexte, options, décision, conséquences).
- Rôle de l'IA : rédiger le brouillon ; **la décision appartient aux humains**.

## La règle qui relie tout : la Pull Request

- Chaque contribution — humaine ou proposée par l'IA — passe par une **PR**.
- Au moins un humain (y-magma ou Vincent) relit et fusionne.
- La relecture vérifie le **respect des règles de fond** (voir [`../AGENTS.md`](../AGENTS.md) et [`../vision/manifeste.md`](../vision/manifeste.md)) : steelman présent, faits/valeurs/hypothèses séparés, incertitudes nommées.
- Rien n'est jamais « définitif » : un document peut être rouvert, amendé, ou marqué obsolète tout en restant dans l'historique.

## Rythme suggéré

- **En continu** : dépôt d'idées et de points de vue.
- **Par sessions** (seul, à deux, ou avec l'IA) : on choisit une idée chaude, on la confronte, on la synthétise.
- **Ponctuellement** : on distille les slogans mûrs et on consigne les décisions.
