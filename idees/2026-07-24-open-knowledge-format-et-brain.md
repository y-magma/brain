# Idée : Open Knowledge Format (OKF) — format d'échange utile, ou distraction pour l'atelier ?

- **Date** : 2026-07-24
- **Proposé par** : IA (à partir d'une question de y-magma)
- **Statut** : graine · en débat
- **Échelle(s)** : individu · communauté · société

## La graine

Pour un futur **outil grand public** (et pour la recherche collaborative à deux qui cherche la forme d'une « machine à penser »), faut-il adopter le **Open Knowledge Format (OKF)** de Google Cloud — un format ouvert Markdown + YAML frontmatter conçu pour que humains et agents IA partagent la même base de connaissance ?

Intuition à tester : **ce n'est pas un oui/non unique.** OKF formalise un motif que `brain` pratique déjà (wiki de Markdown versionné, lisible par humains et IA). Mais OKF vise surtout l'**interopérabilité de catalogues de connaissance** (schémas, métriques, runbooks, contexte d'agents) — pas encore le modèle éditorial de `brain` (idées, steelman, multi-échelle, divergences assumées).

Hypothèse de travail : distinguer deux couches —

1. **L'atelier de recherche** (ce dépôt, 2 personnes + IA) : prioriser le *contenu du raisonnement* et le cycle en cinq temps ; OKF n'est pas une condition pour avancer.
2. **Le produit grand public** (s'il émerge) : OKF (ou un format voisin) peut devenir pertinent comme **couche d'échange** si l'outil doit parler à plusieurs agents / outils sans se lier à une plateforme.

## Pourquoi ça compte

- Évite de confondre **format d'infrastructure** et **forme de démocratie** (deux problèmes différents).
- Évite de perdre du temps à « se mettre au standard » avant d'avoir clarifié ce qu'on veut construire.
- Évite aussi l'angle mort inverse : ignorer un standard naissant alors que `brain` est déjà un cousin du motif « LLM-wiki » que OKF cherche à unifier.

## Ce qu'on ne sait pas encore

- OKF v0.1 est-il assez stable et adopté hors Google Cloud pour être un pari raisonnable ?
- Notre modèle (faits / valeurs / hypothèses, convergences / divergences) a-t-il besoin de champs structurés au-delà de `type` + Markdown libre ?
- Le produit grand public doit-il *exporter* de la connaissance (export OKF) ou seulement *faire vivre* un débat pour des humains ?
- Faut-il se rapprocher d'OKF *maintenant* (frontmatter minimal), *plus tard*, ou *jamais* (format maison + export éventuel) ?

## Nature des énoncés (à préciser)

- **Faits** (vérifiables) :
  - OKF (annoncé juin 2026, Google Cloud) décrit un bundle = répertoire de fichiers Markdown avec YAML frontmatter ; le seul champ obligatoire est `type` ; format vendor-neutral, pas une plateforme.
  - `brain` est déjà un dépôt de Markdown versionné par Git, avec gabarits et liens relatifs — proche du motif « LLM-wiki », sans frontmatter YAML ni conformité OKF.
  - OKF n'est pas schema.org (balisage web public) ni un signal SEO direct ; c'est une couche de données pour agents / catalogues.
- **Valeurs** (choix moraux/politiques) :
  - Préférer l'ouverture et la non-capture par un vendor, sans pour autant adopter un format par effet d'autorité (« Google l'a publié »).
  - Le fond (qualité du débat, pluralisme) prime sur l'infra tant que la forme de l'outil n'est pas claire.
- **Hypothèses** (paris incertains) :
  - Une adoption précoce d'OKF sur `brain` apporterait peu de valeur à deux personnes tant que le *modèle de pensée* n'est pas stabilisé.
  - Une *veille active* + une éventuelle couche d'export (quand un produit existe) pourrait capturer l'avantage d'interopérabilité sans freiner la recherche.

## Liens

- Idée fondatrice : [`2026-07-23-un-outil-de-democratie.md`](2026-07-23-un-outil-de-democratie.md)
- Débat associé : [`../points-de-vue/2026-07-24-adopter-okf-maintenant.md`](../points-de-vue/2026-07-24-adopter-okf-maintenant.md)
- Vision : [`../vision/manifeste.md`](../vision/manifeste.md)
- Source externe (à relire) : [annonce OKF — Google Cloud Blog](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing) · [spéc / repo](https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf)
